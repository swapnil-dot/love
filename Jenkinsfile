pipeline {
    agent {
        docker { image 'swapy25/maven' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'mvn --version'
                node {
  
                      docker.image('swapy25/maven').withRun {c ->
                          sh 'mvn --version'
                     }
                 }
            }
        }
    }
}
