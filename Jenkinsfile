pipeline{
    agent any
    stages{
        stage("Go Build") {
            agent { docker { image 'golang' } }
            steps{
                dir('./src'){
                    sh 'go get github.com/gorilla/websocket'
                }
            }
        }  
        stage("Go run"){
            steps{
                dir('./src'){
                    sh 'go get github.com/gorilla/websocket'
                    sh 'go run main.go'
                }
            }
        }
    }
}
