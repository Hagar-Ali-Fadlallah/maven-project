pipeline {
    agent any 
    tools { 
      maven 'MAVEN_HOME' 
      jdk 'openjdk-11' 
    }
    stages {
        stage('clone repo and clean') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
