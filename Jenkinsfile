pipeline {
    agent any
    stages {
        stage('permision') { 
            steps {
                sh 'chmod +x ./script.sh'
                }
        }
        stage('failed'){
            steps{
                sh 'exit 1'
            }
        }
        stage('execution'){
            steps{
                sh './script.sh'
            }
        }
    }
}
