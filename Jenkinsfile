pipeline {
    agent { docker { image 'golang' } }    
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
