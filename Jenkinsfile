pipeline {
  agent any
  
  stages {
    stage('Clone Repo') {
      steps {
        echo "Cloning the project"
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
      }
    }

    
  }
}
