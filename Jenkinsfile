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
        dockerNode(image: 'ubuntu') {
          sh 'echo sajt'
        }

      }
    }

  }
}