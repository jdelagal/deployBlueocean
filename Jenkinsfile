pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:/root'
        sh 'docker exec -i toolkit_running bash'
      }
    }
    stage('Exec') {
      steps {
        sh '''
          echo "yes" | ./apic.sh && echo "no" | ./apic.sh
        '''
      }
    }
  }
}