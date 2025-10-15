pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checking out...'
        checkout scm
      }
    }
    stage('Install / Verify') {
      steps {
        // prints python version and lists workspace (Windows)
        bat 'python --version'
        bat 'dir'
      }
    }
    stage('Run') {
      steps {
        // run your python app
        bat 'python app.py'
      }
    }
  }
}
