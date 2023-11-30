pipeline {
  agent any
  stages {
    stage('Ubuntu Stage') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        script {
          sh 'uname -a'
        }

      }
    }

    stage('Alpine Stage') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        script {
          sh 'uname -a'
        }

      }
    }

  }
}