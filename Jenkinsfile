pipeline {
    agent {
        docker {
            image 'node:16'
            args '-u root'
        }
    }
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'npm install --save'
            }
        }
    }
    
    post {
        success {
            echo 'Successed'
        }
        failure {
            echo 'Failed'
        }
    }
}
