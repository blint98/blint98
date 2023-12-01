pipeline {
  agent any
  stages {
    stage('Ubuntu Stage') {
      agent {
        docker {
          image 'ubuntu'
          args '-v /var/run/docker.sock:/var/run/docker.sock -v /usr/bin/docker:/usr/bin/docker --privileged'
        }

      }
      steps {
        script {
          sh 'uname -a'
          sh' apt install docker.io'
        }

      }
    }

    stage('Alpine Stage') {
      agent {
        docker {
          image 'alpine'
          args '-v /var/run/docker.sock:/var/run/docker.sock -v /usr/bin/docker:/usr/bin/docker --privileged'
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