pipeline {
  agent any

  environment {
    Docker_Image_Name = 'athithyanac/app'
  }
  
  stages {
    parallel {
      
        stage('Git Verify') {
          steps {
            sh 'git --version'
          }
        }   
      stage('Docker Verify') {
        steps {
          sh 'docker --version'
         }
       }
    }
    stage('Docker build') {
      steps {
        sh "docker build -t ${Docker_Image_Name}:${env.BUILD_NUMBER} ."
      }
    } 
  }
}

  