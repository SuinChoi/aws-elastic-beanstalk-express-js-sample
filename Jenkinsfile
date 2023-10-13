pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                tool name: 'NodeJs', type: 'ToolType'
                sh 'npm install'
            }
        }
    }
    
    post {
        success {
            echo 'Succeeded'
        }
        failure {
            echo 'Failed'
        }
    }
}
