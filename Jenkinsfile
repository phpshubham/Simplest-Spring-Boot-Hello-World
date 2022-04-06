pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/bratzelk/spring-boot-hello-world.git'
            }
        }
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }    
        stage('Maven Build'){
            steps{
                sh 'mvn package'
            }
        }    
        stage('Deploy'){
            steps{
                sh 'Deploying to server'
            }
        } 
    }
}
