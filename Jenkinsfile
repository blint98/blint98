pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        sh 'echo "Hello world"'
      }
    }

    stage('docker') {
      steps {
        dockerNode(image: 'ubuntu') {
          sh '''apt install python3 -y 
apt install docker-compose -y '''
        }

      }
    }

  }
}