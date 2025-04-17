pipeline {
    agent { 
        node {
            label 'docker-agent-node'
            }
      }
    stages {
        stage('Install dependencies') { 
            steps {
                sh "chmod +x install_deps.sh"
                sh "./install_deps.sh"
            }
        }
        stage('Build') { 
            steps {
                sh "chmod +x build.sh"
                sh "./build.sh"
            }
        }
    }
}