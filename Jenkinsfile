pipeline {
  agent {
    docker {
     image 'kafebob/rpi-alpine-node'
     args '-p 3000:3000'
    }
    stages { stage('Build') { steps { sh 'npm install' } } } 
}
}
