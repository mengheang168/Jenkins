pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building application'
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
      steps {
        echo 'Deploy application'
      }
    }

  }
}