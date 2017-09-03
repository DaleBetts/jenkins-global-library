pipeline {
  agent any
  stages {
    stage ('Git commit ref') {
      steps {
        echo "My Branch NAme: ${env.BRANCH_NAME}"
        script {
          def myLib = new linuxacademy.git.gitStuff();

          echo "My Commit: ${myLib.gitCommit("${env.WORKSPACE}/.git")}"
          sayHello 'dale'
          echo "test"
        }
      }
    }
  }
}
