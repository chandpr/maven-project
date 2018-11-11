pipeline {
    agent any
    stages{
        stage('Building..'){
            steps{
                bat 'mvn clean package'
                bat 'docker build ./Dockerfile -t tomcatwebapp:${env.BUILD_ID}'
            }            
        }
    }
}