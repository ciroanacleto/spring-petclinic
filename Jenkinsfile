pipeline {
  agent {
    docker {
      image 'openjdk:8-jdk'
    }

  }
  stages {
    stage('java') {
      steps {
        sh './mvnw install'
      }
    }
    stage('run') {
      steps {
        sh 'pwd'
        sh './mvnw spring-boot:run'
      }
    }
  }
}