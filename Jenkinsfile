pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('build:...!') {
            steps {
                sh 'go version'
                sh 'go /src/main.go'
            }
        }
    }
}
