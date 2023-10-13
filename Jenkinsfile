pipeline {
    agent {
        docker {
            image 'node:16'  // Specify the Node.js 16 Docker image
            args '-v /var/run/docker.sock:/var/run/docker.sock'  // Optional: Mount Docker socket
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'  // Your build steps go here
            }
        }
    }
}
