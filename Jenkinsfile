pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:.'
        sh 'docker exec -i toolkit_running bash'
        sh 'ls -ltr'
      }
    }
  }
}