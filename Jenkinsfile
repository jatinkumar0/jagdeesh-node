pipeline {
agent any
  stages{
  
    stage('Build'){
      steps {
      sh 'npm install'
      }
    }
    
    stage('Deploy'){
      steps{
      sh 'pm2 delete all'
      sh 'pm2 start index.js'
      }
    }
  
  }
}
