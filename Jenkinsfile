pipeline {
  agent any
  stages {
    stage('list file') {
      steps {
        sh "ls -la"
      }
    }

    stage('Clean Build') {
      steps {
        sh "mvn clean"
        echo "list all files"
      }
      steps {
        sh "ls -la"
        sh "tree"
      }
    }
  }
}