pipeline 
{
  agent any
  stages 
  {
    stage('list file') 
    {
      steps 
      {
        sh "ls -la"
      }
    }  
    stage('clean build') 
    {
      steps 
      {
        sh "mvn clean"
        sh 'ls -la'
        sh "tree"
      }
    }
    stage('Generate build') 
    {
      steps 
      {
        sh "mvn install"
        sh 'ls -la'
        sh 'tree'
      }
    }
  
  }
}