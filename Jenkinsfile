 pipeline {
    agent any

    stages {
        stage('pull') {
            steps {
                git credentialsId: 'Kumarazdevops' , url: 'https://github.com/Kumarazdevops/docker_task.git'
            }
        }
        stage('Build') {
            steps{
                bat 'docker build -t taskimage .'
            }
        }
    }
 }
