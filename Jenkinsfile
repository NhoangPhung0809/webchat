pipeline {
    agent any
    tools {
        go 'go-1.17'
    }
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
