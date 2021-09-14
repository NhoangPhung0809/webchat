pipeline {
    agent { docker { image 'golang' } }    
    environment {
         GO117MODULE = 'on'
    }
    stages {
        stage('bul') {
            steps {
                sh 'go run /src/main.go'
            }
        }
    }
}
