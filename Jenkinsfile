pipeline {
    agent any
    stages {
            stage('Install Node.js') {
                steps {
                    sh 'apt-get update && apt-get install -y nodejs npm'
                }
            }
            stage('List file in root app folder') {
                steps {
                    sh 'ls -la' // List files in the 'app' directory
                }
            }
            stage('List file in views app folder') {
                steps {
                    sh 'ls -la views' // List files in the 'app/views' directory
                }
            }
            stage('Test') {
                steps {
                    sh 'npm install && npm run test'
                }
            }
    }
}
