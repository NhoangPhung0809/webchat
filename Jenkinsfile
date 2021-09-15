pipeline {
    agent { docker { image 'golang' } }
    stages{
     stage('Start') {
        steps {
               sh './build.sh'
               sh 'go version'
               sh 'cd ./src'
         }
    }
        stage('build') {
            steps {
                sh 'go get github.com/gorilla/websocket'
                echo 'Build...!....!'
                sh 'go run ./src/main.go'
            }
        }
    }
}
