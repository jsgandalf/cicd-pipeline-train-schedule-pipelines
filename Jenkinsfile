pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running Build automation'
        sh './gradle build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
