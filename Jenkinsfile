pipeline { 
	 agent { 
	 docker {
	 	image 'kafebob/rpi-alpine-node' 
		args '-u root:root -p 3000:3000 -v "$HOME":/home'
		}
		} 
		stages {
		  stage('Build') { 
		  steps {
		   sh 'npm install' 
		   } 
		   } 
		   } 
}
