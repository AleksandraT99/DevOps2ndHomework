pipeline {
    agent { docker { image 'maven:3.6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
