pipeline {
  agent {
    node {
      label 'slave1'
    }

  }
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/DomAbin/Devops_demo.git'
      }
    }

    stage('Publish') {
      steps {
        bat 'echo "hello"'
      }
    }

    stage('Post') {
      steps {
        powershell 'echo "success"'
      }
    }

  }
}