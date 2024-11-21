pipeline {
    agent {
        label 'AGENT-1'
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
    post {
        always{
            echo "This section always runs"
            deleteDir()
        }
        success{
            echo "This section runs when pipeline success"
        }
        failure{
            echo "This section run ehn pipeline failure"
        }
    }
}