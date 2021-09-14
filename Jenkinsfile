pipeline {
    agent any
    tools {
        go 'go-1.16'
    }
   environment {
        GO116MODULE = 'on'
        CGO_ENABLED = 0 
   }
    stages {     
        stage('Pre Test') {
            steps {
                echo 'Installing dependencies'
                sh 'go version'
                sh 'go get -u golang.org/x/lint/golint'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling and building'
                sh 'go build'
            }
        }
        stage('build') {
            steps {
                sh "chmod +x -R ${env.WORKSPACE}"
                sh 'go run main.go'
            }
        }
    }
}
