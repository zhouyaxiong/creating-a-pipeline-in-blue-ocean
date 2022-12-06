pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'build\''
        echo '${username}'
      }
    }

    stage('Test') {
      steps {
        echo 'test success'
      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy success'
      }
    }

  }
  environment {
    username = 'jenkins'
  }
}