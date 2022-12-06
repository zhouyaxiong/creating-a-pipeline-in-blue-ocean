pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
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

        stage('build2') {
          steps {
            echo '${username}'
          }
        }

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