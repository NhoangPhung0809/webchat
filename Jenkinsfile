pipeline {
    agent { docker { image 'golang' } }
    environment {
        module 'websocket'
    }
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
