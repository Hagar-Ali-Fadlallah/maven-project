pipeline {
    agent any 
    tools { 
      maven 'MAVEN_HOME' 
      jdk 'openjdk-11' 
    }
    stages {
        stage('clone repo and clean') { 
            steps {
                echo "-------------cleaning------------"
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
                echo "------------------Deploying in linux Environment--------------"
                sh "mvn package"
            }
        }
        stage('Document') { 
            steps {
                echo "------------------This is documentation part--------------"
               
            }
        }
    }
}
