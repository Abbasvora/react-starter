pipeline {
    agent { 
        node {
            label 'docker-agent-node'
            }
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