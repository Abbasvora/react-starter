pipeline {
    agent {
        docker {image: 'node:16-alpine'}
    }
    tools{
        nodejs 'nodejs'
    }
    stages {
        stage('Install dependencies') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('Build') { 
            steps {
                sh 'npm run build' 
            }
        }
    }
}