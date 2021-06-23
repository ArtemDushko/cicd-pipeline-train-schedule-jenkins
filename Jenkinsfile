pipeline {
  agent any
  stages {
    steps ('Build') {
      echo 'Running build automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
