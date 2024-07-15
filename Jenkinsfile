pipelin {
  agent any

  stages{
    stage('clone'){
      steps{
        git branch : 'main', url: 't https://github.com/Kumarazdevops/docker_task.git'
      }
    }
    stage('Build image'){
      steps{
        sh 'docker build -t myimage2 .'
      }
    }
  }
}
