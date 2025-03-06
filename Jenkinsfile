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
                sh 'docker build -t web'
            }
        }
    }
}