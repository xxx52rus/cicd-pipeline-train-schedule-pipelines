pipeline {
  agent any
  stages {
    stage {'build'} {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainShedule.zip'
      }
    }
  }
}
