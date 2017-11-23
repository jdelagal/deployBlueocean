pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -i toolkit_running bash'
      }
    }
  }
}