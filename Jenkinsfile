pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                echo "this is building stage"
            }
        }
        stage("test") {
            steps {
                sh 'exit 1' // This command will cause the pipeline to fail
            }
        }
        stage ("delever"){
            steps{
                echo "this is deply"
            }
        } 
        stage ("deply"){
            steps{
                echo "this is deply"
            }
        } 
        
        
    }
}

