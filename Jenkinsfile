pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/AantNrayn/BoardgameListingWebApp.git'
            }
        }
        
                stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        
                stage('Test') {
            steps {
                sh 'mvn clean test'
            }
        }
        
                stage('package') {
            steps {
                sh 'mvn clean package'
            }
        }
        
                stage('Docker') {
            steps {
                echo 'docker started'
            }
        }
        
    }
}
