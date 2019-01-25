pipeline { 
	 agent { 
	 docker {
	 	image 'kafebob/rpi-alpine-node' 
		args '-p 3000:3000'
		}
		} 
		stages {
		  stage('Build') { 
		  steps {
		   sh 'whoami'
		   sh 'sudo chown -R root:root /.config'
		   sh 'npm install' 
		   } 
		   } 
		   } 
}
