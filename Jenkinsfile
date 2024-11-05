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

        stage('') {
          steps {
            echo 'API Testing'
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