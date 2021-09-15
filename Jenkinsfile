pipeline {
    agent { docker { image 'golang' } }
    
    stage('Start') {
         echo 'Start....'
         withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin", "GOBIN=${root}/bin", "GOPATH=${root}/go"]) {
         sh 'go version'
      steps {
               sh './build.sh'
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
