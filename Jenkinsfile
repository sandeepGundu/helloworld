pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'echo \'Building\''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Echo \'Testing\''
          }
        }

        stage('Test2') {
          steps {
            echo 'hello'
          }
        }

      }
    }

    stage('Archive') {
      steps {
        echo 'echo \'Archiving\''
      }
    }

  }
}