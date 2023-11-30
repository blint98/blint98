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
        sh '''apt install docker.io -y 
docker run ubuntu'''
      }
    }

  }
}