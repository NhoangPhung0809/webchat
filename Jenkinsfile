pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Start') {
            steps {
                sh 'go version'
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
