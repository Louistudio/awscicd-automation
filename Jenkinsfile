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
                'TRIVY', target: '.', format: 'table', severity: 'HIGH,CRITICAL'
            }
        }    
        stage('codescan'){
            steps{
                sh 'trivy --version'
            }
        }
    }
}