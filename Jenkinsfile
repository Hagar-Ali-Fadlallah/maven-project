pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/Hagar-Ali-Fadlallah/maven-project', branch: 'main')
      }
    }

    stage('Printing message ') {
      steps {
        sh 'echo "success"'
      }
    }

  }
}