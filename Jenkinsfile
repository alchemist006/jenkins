pipeline {
    agent any
    
    tools {nodejs "NodeJs 16.x"}
    
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/alchemist006/jenkins'
            }
        }
        stage('Install Dependencies'){
            steps {
                sh 'npm install'
            }
        }
        stage ('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}