pipeline {
    agent {
        docker { image 'swapy25/maven' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                docker.image('swapy25/maven').withRun {c ->
                     sh 'mvn --version'
                 }
            }
        }
    }
}
