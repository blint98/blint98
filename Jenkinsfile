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
          sh '''sudo apt install docker.io
docker run -d ubuntu'''
        }

      }
    }

  }
}