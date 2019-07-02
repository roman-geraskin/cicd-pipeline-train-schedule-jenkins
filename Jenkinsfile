pipeline {
  agent any
  stages {
    stage ('Build') {
      echo "Starting automated build"
      sh "./gradlew build --no-daemon"
      archiveArtifacts artifacts: dist/trainSchedule.zip
    }
  }
}
