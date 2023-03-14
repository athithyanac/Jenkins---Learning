pipeline {
  agent any
  
  stages {
    stage ('Git Verify') {
      steps {
        sh 'git --version'
	    }
    }
   stage ('Docker Verify') {
    steps {
      sh 'docker --version'
    }
   }
  }
}


