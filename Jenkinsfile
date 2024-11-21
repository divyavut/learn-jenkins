pipeline {
    agent {
        label 'AGENT-1'
    }
    
    tools {
    nodejs 'NodeJS'  // Ensure 'NodeJS' matches the name in Global Tool Configuration
    }
    stages {
        
        stage('Build') { 
            steps {
               sh 'echo "this is the build"'
            }
        }
        stage('Test') { 
            steps {
               sh 'echo "this is the test"'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo "this is the deploy"'
            }
        }
    }
}