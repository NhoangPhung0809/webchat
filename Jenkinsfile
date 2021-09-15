pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Start') {
            steps {
                def root = tool name: '1.8.3', type: 'go'
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
