pipeline {
    agent any
    environment {
        PATH = "$PATH:/home/administrator/.nvm/versions/node/v20.0.0/bin" // replace /path/to/npm with the actual path to the npm command
    }
    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run tests') {
            steps {
                sh 'npm run android'
            }
        }
    }
}