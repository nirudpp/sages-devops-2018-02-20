pipeline {
  agent any
  stages {
    stage('Pull Request') {
      when {
               branch 'nirudpp' | 'feature'
            }
      steps {
        sh "echo ${env.GIT_BRANCH}"
      }
    }
  }
}
