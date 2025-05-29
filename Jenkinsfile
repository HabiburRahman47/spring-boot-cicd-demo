pipeline {
  agent any

  tools {
    maven 'MAVEN'
    jdk 'JAVA_HOME'
  }
  
  stages {
    stage('Clone Repo') {
      steps {
        echo "Cloning the project"
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo "Building the project"
        sh 'mvn clean install'
      }
    }

    stage('Test') {
      steps {
        echo "Testing the project"
        sh 'mvn test'
      }
    }

    
  }
}
