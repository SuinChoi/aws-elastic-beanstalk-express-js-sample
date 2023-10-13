pipeline {
    agent any
    tools {
        nodejs 'NodeJS'
    }
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!'
            }
        }
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
}
