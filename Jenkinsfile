pipeline {
  agent any


  environment {
        DOCKER_IMAGE = 'myimage:latest'
    }

  stages{
    stage('clone'){
      steps{
        git branch : 'master', url: 'https://github.com/Kumarazdevops/docker_task.git'
      }
    }
    stage('Build image'){
      steps{
        bat 'docker built -t myimage .'
        echo "build image"
      }
    }
  }
}
