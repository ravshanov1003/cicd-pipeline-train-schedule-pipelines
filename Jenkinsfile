pipeline{
  agent any
  stages {
    stage ('Build'){
      steps{
        echo 'Running build automation'
        sh 'gradle wrapper --gradle-version 5.1 \
        ./gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
