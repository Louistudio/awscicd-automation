pipeline{
    agent {
        docker {
            image 'docker:dind'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }


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
    }
}