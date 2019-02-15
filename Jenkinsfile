pipeline {
	agent any
	
	stages {
		
		stage('Deploy to Local') {
			steps {
				/*
				//shell script will not work in jenkins running on windows
				sh '''
				echo "PATH=${PATH}"
				echo "M2_HOME=${M2_HOME}"
				'''
				*/
				echo "%PATH%"
			}
		}
		
		stage('Deploy to Prod') {
			steps {
				echo "hello world, prod deploy"
			}
		}
	}
}