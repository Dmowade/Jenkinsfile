pipeline {
  agent any
  stages {
    stage('buils stage') {
      steps {
        sh 'date'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I am here'
          }
        }

        stage('Test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Hi Jenkins'
        sleep 10
      }
    }

  }
}