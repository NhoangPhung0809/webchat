pipeline{
    agent any
    stages{
        stage("Go Build") {
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
        stage(GO stop){
            steps{ 
                dir('./src'){
                    sh 'go stop'
                }
            }
        }
    }
}
