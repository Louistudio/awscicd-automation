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
                sh 'uname -r'
            }
        }
        stage('codescan'){
            steps{
                sh 'apt install trivy'
            }
        }
    }
}