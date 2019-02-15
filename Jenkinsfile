pipeline {
	agent any
	
	stages {
		
		stage('Deploy to Local') {
			steps {
				sh '''
				echo "PATH=${PATH}"
				echo "M2_HOME=${M2_HOME}"
				'''
			}
		}
		
		stage('Deploy to Prod') {
			steps {
				echo "hello world, prod deploy"
			}
		}
	}
}