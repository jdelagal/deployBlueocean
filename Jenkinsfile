pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:/root'
        sh 'docker exec -i toolkit_running bash'
        sh 'chmod 775 apic.sh'
        sh 'ls -ltr'
      }
    }

    stage('Exec') {
      steps {
        sh 'echo "yes"'
        sh 'pwd'
      }
    }
  }
}