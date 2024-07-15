pipelin {
  agent any

  stages{
    stage('clone'){
      steps{
        git branch : 'main', url: 'https://github.com/Kumarazdevops/docker_task.git'
      }
    }
    stage('Build image'){
      steps{
        bat 'docker build -t myimage2 .'
      }
    }
  }
}
