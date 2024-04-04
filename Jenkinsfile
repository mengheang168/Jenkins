pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Building application'
          }
        }

        stage('build1') {
          steps {
            echo 'building one'
          }
        }

        stage('build2') {
          steps {
            echo 'building two'
          }
        }

      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing application'
          }
        }

        stage('checking') {
          steps {
            echo 'Checking Application'
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Deploy application'
          }
        }

        stage('testing before deploy') {
          steps {
            echo 'Testing'
          }
        }

      }
    }

    stage('Deploy 1') {
      steps {
        echo 'Deploy one'
      }
    }

    stage('Deploy 2') {
      steps {
        echo 'Deploy 2'
      }
    }

    stage('Deploy 3') {
      steps {
        echo 'Deploy 3'
      }
    }

  }
}