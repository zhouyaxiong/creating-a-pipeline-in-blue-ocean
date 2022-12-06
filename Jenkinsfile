pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      environment {
        username = 'zhouyx'
      }
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
        catchError()
      }
    }

  }
  environment {
    username = 'jenkins'
  }
}