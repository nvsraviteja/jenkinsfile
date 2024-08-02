pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'chmod +x ./script.sh'
                sh './script.sh'
            }
        }
    }
}
