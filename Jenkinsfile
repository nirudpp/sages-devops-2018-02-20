pipeline {
  agent any
  stages {
    stage('Pull Request') {
      when {
               branch 'nirudpp'
            }
      steps {
        sh "echo ${env.GIT_BRANCH}"
      }
    }
  }
}
