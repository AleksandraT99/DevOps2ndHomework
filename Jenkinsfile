pipeline {
    agent any 
    stages {
 
        stage('Build') {
            steps {
                sh 'make' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }     
        }
        
        stage('Test phase') {
            steps {
                echo 'Hello world!' 
            }
        }
    }
}
