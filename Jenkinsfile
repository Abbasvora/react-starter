pipeline {
    agent { 
        node {
            label 'docker-agent-node'
            }
      }
    stages {
        stage('Install dependencies') { 
            steps {
                sh -c 'npm -v'
                sh -c 'npm install' 
            }
        }
        stage('Build') { 
            steps {
                sh 'npm run build' 
            }
        }
    }
}