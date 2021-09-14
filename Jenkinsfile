pipeline {
    agent any
    tools {
        go 'go-1.11'
    }
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
