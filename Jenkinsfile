pipeline {

agent none

stages {
  stage ('build') {
      
steps {
      sh 'docker build -t my-hello-world:v1 .'
    }
   }

stage ('Test1') {
steps {
sh 'docker images'
}
}

stage ('Run') {
steps {
sh 'docker run -d -p 5000:5000 my-hello-world:v1'
}
}
stage ('Test2') {
steps {
sh 'docker ps'
}
}


stage ('Test App') {
steps {
sh 'curl http://127.0.0.1:5000'
}
}

}

}
