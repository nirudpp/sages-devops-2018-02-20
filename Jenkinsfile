pipeline {
  agent any
  stages {
    stage('Pull Request') {
      when {
        anyOf {
          environment name: 'GIT_BRANCH', value: 'nirudpp'
          environment name: 'GIT_BRANCH', value: 'feature'
        }
        
      }
      steps {
        sh "echo ${env.GIT_BRANCH}"
      }
    }
    stage('Sonar') {
      steps {
        waitForQualityGate()
      }
    }
  }
}