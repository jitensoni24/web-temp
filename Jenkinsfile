pipeline {
	agent any
	
	stages {
		
		stage('Initial test message') {
			steps {
				echo "checking stage: hello world: jenkins pipeline"
			}
		}

		stage('Package war file') {
			steps {
				echo "Building war file with maven..."
			
				//bat for windows to execute script files else use sh'''
				bat 'mvn clean package'
			}
			post {
				success {
					echo 'now archiving war file'

					archiveArtifacts artifacts: "**/*.war"
				}

			}
		}

		stage('Deploy to Local') {
			steps {
				build job: 'deploy-local'
			}
		}		
	}
}