pipeline {
    agent any
    stages {
        stage('permision') { 
            steps {
                sh 'chmod +x ./script.sh'
            }
            stage('execution'){
                sh './script.sh'
            }
        }
    }
}
