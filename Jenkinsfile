pipeline{
    agent {docker {images 'ubuntu'}}
    stages{
        stage("Go Build.!.!.!"){
            steps{
                dir('./src') {
                    sh 'go get github.com/gorilla/websocket'
                }
            }
        }
         stage("Testing.!.!.!"){
            steps{
                dir('./src') {
                    sh 'go stop'
                }
            }
         }
    }
}
