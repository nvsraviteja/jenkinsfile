pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                chmod +x ./script.sh
                sh ./script.sh
            }
        }

    }
}

