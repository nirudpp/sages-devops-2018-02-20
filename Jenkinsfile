pipeline {
  agent any
  stages {
    stage('Pull Request') {
      when {
                expression { BRANCH_NAME ==~ /(nirudpp|feature|hotfix|bugfix)/ }
            }
      steps {
        sh 'echo ${env.GIT_BRANCH}'
      }
    }
  }
}
