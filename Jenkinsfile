pipeline {
    agent any
    environment {
         GO117MODULE = 'on'
    }
    stages {
        stage('buil') {
            steps {
                sh 'go run ./src/main'
            }
        }
    }
}
