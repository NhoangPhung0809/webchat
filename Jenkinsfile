pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Start') {
            steps {
                echo 'Start....'
                sh 'go version'
                sh 'cd ./src/'
            }
        }
        stage('Module') {
            steps {
                echo 'Module...!....!'
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
