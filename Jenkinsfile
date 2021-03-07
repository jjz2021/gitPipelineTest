pipeline {
  environment {
    imagename = "jjjz2021/gitPipelineTest"
    registryCredential = 'docker-hub'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git([url: 'git@github.com:jjz2021/gitPipelineTest.git', branch: 'main', credentialsId: 'gitHub-SSH'])
      }
    }
    stage('Deploy image and Remove Unused  image') {
      steps{
        sh "docker --version"
      }
    }
  } 
}    
