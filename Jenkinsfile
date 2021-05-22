pipeline {
    node("linux_server") {

        stage('Pull') {
                git 'https://github.com/GaraninR/JenkinsDotnet.git'
        }

        stage('Build') {
                sh 'dotnet build'
        }

        stage('Test') {
                sh 'dotnet test'
        }
            
    }
}