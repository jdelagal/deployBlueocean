pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -i -u root toolkit_running test "apic -ht"'
      }
    }
  }
}