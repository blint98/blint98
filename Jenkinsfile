pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        sh 'echo "Hello world"'
      }
    }

    stage('kövi') {
      steps {
        sh '''sudo apt install docker.io -y 
docker run ubuntu'''
      }
    }

  }
}