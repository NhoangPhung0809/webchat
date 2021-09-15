pipeline {
    agent { docker { image 'golang' } }
    stages {
        withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin", "GOBIN=${root}/bin", "GOPATH=${root}/go"]) {
        sh 'go version'
        sh './build.sh'
        }
    }
        stage('Start') {
            steps {
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
