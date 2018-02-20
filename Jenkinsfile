pipeline {
  agent any
  stages {
    stage('Kompilacja') {
      steps {
        sh 'echo \'mvn build\''
      }
    }
    stage('Unit Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo \'test\''
            echo 'test 2'
          }
        }
        stage('UI Test') {
          steps {
            echo 'UI test'
          }
        }
      }
    }
    stage('Publish to Artifactory') {
      steps {
        echo 'artifactory'
      }
    }
  }
}