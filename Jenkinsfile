pipeline {
  agent {
    node {
      label 'node'
    }

  }
  stages {
    stage('1') {
      steps {
        sh 'echo build'
      }
    }

    stage('2') {
      parallel {
        stage('2') {
          steps {
            echo 'message'
          }
        }

        stage('3') {
          steps {
            echo '1'
          }
        }

        stage('') {
          steps {
            echo '333'
          }
        }

        stage('5') {
          steps {
            echo '3'
          }
        }

      }
    }

  }
  environment {
    jenkins = 'jenksni'
  }
}