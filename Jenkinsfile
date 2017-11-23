pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:.'
        sh 'docker exec -i toolkit_running bash'
        sh 'chmod 775 apic.sh'
        sh 'ls -ltr'
        sh 'echo "yes" | ./apic.sh'
      }
    }
  }
}