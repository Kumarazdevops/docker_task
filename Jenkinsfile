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
                bat 'docker run -d --name taskcount -p 8072:80 taskimage'
            }
        }
    }
 }
