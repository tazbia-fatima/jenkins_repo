pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'go build hello.go'
        sh 'ls'
        } 
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
 }
}




