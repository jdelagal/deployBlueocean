pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -ti toolkit_running script /dev/null ls'
      }
    }
  }
}