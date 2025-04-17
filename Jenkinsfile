pipeline {
    agent { 
        node {
            label 'docker-agent-node'
            }
      }
    stages {
        stage('Install dependencies') { 
            steps {
                sh "chmod +x test.sh"
                sh "./test.sh"
            }
        }
        stage('Build') { 
            steps {
                sh 'npm run build' 
            }
        }
    }
}