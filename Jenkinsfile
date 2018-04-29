pipeline {
  agent {
    docker {
      image 'openjdk:8-jdk'
    }

  }
  stages {
    stage('build') {
      steps {
        sh './mvnw install'
      }
    }
  }
}