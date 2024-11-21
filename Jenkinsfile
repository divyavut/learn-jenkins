pipeline {
    agent {
        label 'AGENT-1'
    }
    options { timeout(time: 10, unit: 'SECONDS') }
    stages {
        
        stage('Build') { 
            steps {
               sh 'echo "this is the build"'
               sh 'sleep 10'
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