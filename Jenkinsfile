pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Starting automated build"
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
