pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/vinod-2/HelloWorld-Springboot-App.git'
            }
        }
        
        stage('maven build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Create Dockerimage'){
            steps{
                sh 'sudo docker build  thetips4you/springboot:latest .'
            }
        }
        
    }
}
