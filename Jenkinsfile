pipeline{
    agent any

    stages{
        stage('Clone'){
            steps{
                sh 'pwd'
            }
        }
        stage('Docker-Build'){
            steps{
                sh 'apt-get update && apt-get install -y docker.io'
                sh 'docker --version'
            }
        }
    }
}