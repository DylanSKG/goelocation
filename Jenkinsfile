pipeline {
    
    agent any
    tools{
        maven 'M2_HOME'
    }
    triggers {
   PollSCM '* * * * *'     
    }

    stages {
        stage('maven Package') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
        }
        stage('test') {
            steps {
                echo 'mvn test'
            }
        }
        stage('test') {
            steps {
                echo 'test'
                
            }
        }
        stage('deploy') {
                echo 'deploy'
        
            }
        }
    }

