pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Test Chrome') {
      parallel {
        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome...\''
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge...\''
          }
        }

        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox...\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}