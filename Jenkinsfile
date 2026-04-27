pipeline {

agent none

stages {
  stage ('build') {
    agent {
     docker { image 'python:3.11' }
     }
     steps {
      python3 'app.py'
    }
   }
}
}
