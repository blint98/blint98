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
                    // Docker image előkészítése, az Ubuntu telepítéssel
                    docker.image('ubuntu').inside {
                        // Ubuntu frissítése és a Docker telepítése
                        sh 'apt-get update && apt-get install -y docker.io'
                    }
                }
            }
        }
    }
}
