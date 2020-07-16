pipeline {
    agent {
        docker { image 'swapy25/maven' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'mvn --version'
                Image.run()
            }
        }
    }
}
