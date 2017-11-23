pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        sh 'docker cp apic.sh toolkit_running:/root'
        sh 'docker exec -i toolkit_running bash'
        sh 'cd /root'
        sh 'chmod 775 apic.sh'
        sh 'echo "yes" | ./script.sh && echo "no" | ./script.sh'
      }
    }
  }
}