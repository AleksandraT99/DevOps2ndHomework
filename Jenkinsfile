pipeline {
    agent any 
    stages {
        stage('Test phase') {
            steps {
                echo 'Hello world!' 
            }
        }
        
        stage('JUnit Test') {
            steps {

                sh 'make check || true' 
                junit 'C:\Users\aleks\eclipse-workspace\Random\src\SimpleTest.java' 
            }
        }
    }
}
