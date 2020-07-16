pipeline{
    agent any
    stages{
        stage('Docker-compose'){
           steps{
             sh 'echo "Running docker-compose.yml......setting up containers!"'
              docker.image('swapy25/maven').withRun {c ->
                    sh 'mvn --version'
                }
              }
           }
        
     }
     post{
       always{
           cleanWs()
             }
         }
}
