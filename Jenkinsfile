pipeline {
agent any
 stages {
  stage ('checkout'){
   checkout scm
  }
  stage ('Build'){
   steps {
      echo 'Runnig build Automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/sampleapp.zip'
      }
     }
    }
  }
