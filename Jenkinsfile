pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Test') {
      steps {
        sh "echo building $BRANCH_NAME"
      }
        }
    }
    post {
    success {
      echo " $BRANCH_NAME build is succeeded!"
    }
    failure {
      echo " $BRANCH_NAME build is failed"
    }
    }
}
tmw-ovop-ipr
