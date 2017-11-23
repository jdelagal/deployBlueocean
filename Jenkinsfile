pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -i -u root toolkit_running script -q -c "/bin/bash" /dev/null'
      }
    }
  }
}