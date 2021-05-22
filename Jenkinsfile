pipeline {
    agent linux_server

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