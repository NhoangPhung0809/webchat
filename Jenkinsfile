pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Start') {
            steps {
                sh 'mkdir /.cache'
                echo 'Start....'
                sh 'go version'
                sh 'cd ./src/'
                sh 'go get github.com/gorilla/websocket'
            }
        }
        stage('build') {
            steps {
                echo 'Build...!....!'
                sh 'go run ./src/main.go'
            }
        }
    }
}
