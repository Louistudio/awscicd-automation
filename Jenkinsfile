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
        stage('Trivy Scan') {
            steps {
                'trivy fs . -o result.html'
            }
        }    
        stage('codescan'){
            steps{
                sh 'trivy --version'
            }
        }
    }
}