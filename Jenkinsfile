pipeline {
  agent any
  stages {
    stage('Build & Test') {
      steps {
        sh 'mvn test'
        stash(name: 'report', includes: '**/target/surefire-report')
      }
    }

  }
}