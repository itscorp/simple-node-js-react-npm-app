pipeline { 
	 agent { 
	 docker {
	 	image 'kafebob/rpi-alpine-node' 
		args '-u root:root -p 3000:3000 -v "$HOME":/home'
		}
		environment {
	 	CI = 'true'
		} 
}
		stages {
		  stage('Build') { 
		  steps {
		   sh 'npm install' 
		   } 
		   } 
		   stage('Test') {
		   steps {
		   sh './jenkins/scripts/test.sh'
		   }
		   }
		   } 
}
