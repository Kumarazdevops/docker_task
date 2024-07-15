pipeline {
  agent any

  stages{
    stage('clone'){
      steps{
        git branch : 'master', url: 'https://github.com/Kumarazdevops/docker_task.git'
      }
    }
    stage('Build image'){
      steps{
        script{
        bat 'docker built -t my image .'
        echo "build image"
        }
      }
    }
  }
}
