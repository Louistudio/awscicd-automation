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
                sh 'trivy fs . -o result.html'
            }
        }    
        stage('codescan'){
            steps{
                sh 'trivy --version'
            }
        }
        stage('Run as Root') {
            steps {
                script {
                    sh '''
                        sudo chown -R jenkins:jenkins /path/to/directory
                        sudo chmod -R 755 /path/to/directory
                    '''
                }
            }
        }
    }
}