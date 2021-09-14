pipeline{
    agent { docker { image 'golang' } }
    stages{
        stage("tes") {
            steps{
                sh 'go version'
            }
        }
    }
}
