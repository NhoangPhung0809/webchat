pipeline{
    agent { docker { image 'golang' } }
    stages{
        stage("Bild") {
            steps{
                sh 'go version'
            }
        }
    }
}
