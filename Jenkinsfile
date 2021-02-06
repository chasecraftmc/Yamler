  
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
    jdk 'JDK 14'
  }

  triggers {
    pollSCM('H/1 * * * *')
  }
}