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
		   sh 'sudo chown -R $USER:$(id -gn $USER) /.config'
		   sh 'npm install' 
		   } 
		   } 
		   } 
}
