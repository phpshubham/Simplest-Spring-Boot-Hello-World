pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/phpshubham/Simplest-Spring-Boot-Hello-World.git'
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
                echo 'Deploying to server'
            }
        } 
    }
}
