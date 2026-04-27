pipeline {

agent none

stages {
  stage ('build') {
    agent {
     docker { image 'python:3.11' }
     }
     steps {
      sh 'python3 app.py'
    }
   }
}
}
