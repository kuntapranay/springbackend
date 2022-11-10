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
      }
      steps {
        sh "ls -la"
        echo "list all files"
        sh "tree"
      }
    }
    stage('Generate build') {
      steps {
        sh "mvn install"
      }
      steps {
        sh "ls -la"
        echo "list all files"
        sh "tree"
      }
    }
  }
}