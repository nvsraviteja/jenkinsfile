pipeline {
    agent any
    
    stages {
        stage('permission') {
            steps {
                echo 'Building...'
                sh 'chmod +x ./script.sh'
            }
        }
        
        stage('execute') {
            steps {
                echo 'Testing...'
                // This command will fail because 'exit 1' returns a non-zero exit code
                sh './script.sh'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'exit 1'
            }
        }
    }
    
    post {
        always {
            echo 'This will always run, even if the pipeline fails.'
        }
        success {
            echo 'This will run only if the pipeline succeeds.'
        }
        failure {
            echo 'This will run only if the pipeline fails.'
        }
    }
}
