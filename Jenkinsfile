pipeline{
    agent any
    stages{
        stage("Go run"){
            steps{
                dir('./src') {
                    sh 'go get github.com/gorilla/websocket'
                    sh 'go build main.go'
                }
            }
        }
    }
}
