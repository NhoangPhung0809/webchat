pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Start') {
            steps {
                echo 'Start....'
                sh 'go version'
            }
        }
        stage('Module') {
            steps {
                echo 'Module...!....!'
                git 'github.com/gorilla/websocket'
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
