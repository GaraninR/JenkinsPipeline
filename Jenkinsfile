pipeline {
    agent any

    stages {

        stage('Pull') {
            steps {
                git 'https://github.com/GaraninR/JenkinsDotnet.git'
            }
        }

        stage('Build') {
            steps {
                sh 'dotnet build'
            }
        }

        stage('Test') {
            steps {
                sh 'dotnet test'
            }
        }
        
    }
}