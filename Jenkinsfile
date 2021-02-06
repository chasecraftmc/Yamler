  
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }
  }

  tools {
    maven 'M3'
    jdk 'j8'
  }

  triggers {
    pollSCM('H/1 * * * *')
  }
}