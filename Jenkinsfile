pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:/root'
        sh 'chmod 775 /root/apic.sh'
      }
    }
  }
}