pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Run a coomand') {
      steps {
        sh '''pwd
                      ls
                      cal 
                    '''
      }
    }

    stage('Print Message') {
      parallel {
        stage('Print Message') {
          steps {
            echo 'Hello this is our jenkinsfile'
          }
        }

        stage('Parallel print') {
          steps {
            echo 'Parallel message print'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy to test') {
      steps {
        echo 'Deploying to test...'
      }
    }

    stage('Manual Approval') {
      steps {
        script {
          input message: 'Do you want to proceed?', ok: 'Proceed'
        }

      }
    }

    stage('Deploy to prod') {
      steps {
        echo 'Deploying to prod...'
      }
    }

  }
}