pipeline {
	agent any
	
	stages {
		stage ('Compile Stage') {
		
			steps {
				withMaven(maven : 'LOCALMAVEN') {
					sh 'mvn clean compile'
			
				}
			}
		}
		
		stage ('Testing Stage') {
			steps {
				withMaven(maven : 'LOCALMAVEN') {
					sh 'mvn test'
				}
			}
		}
		
		stage ('Deploy Stage') {
			steps {
				withMaven(maven : 'LOCALMAVEN') {
					sh 'mvn deploy'
				}
			}
		}
		
	}
}
