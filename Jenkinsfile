pipeline {
  agent any
  stages {
    stage('Hello World') {
      steps {
        script {
          echo 'Hello world!'
        }

      }
    }

    stage('Install Docker on Ubuntu') {
      steps {
        script {
          docker.image('ubuntu').inside {
            sh 'apt-get update && apt-get install -y docker.io'
          }
        }

      }
    }

  }
}