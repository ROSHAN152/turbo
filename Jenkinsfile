pipeline {
  agent any
    
    stage('Build') {
      steps {
        sh 'make check'
        junit 'reports/**/*.xml'
      }
    }
    stage('Test') {
      steps {
        sh 'make publish'
      }
    }
    stage('Deploy') {
      steps {
        sh 'make publish'
      }
    }
  }
}
