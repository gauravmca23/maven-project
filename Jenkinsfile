pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                sh '/usr/local/bin/mvn clean package'
                sh "sudo /usr/local/bin/docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}            
