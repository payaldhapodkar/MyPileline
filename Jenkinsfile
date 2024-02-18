pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Here you would put commands to build your project
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
            steps {
               echo 'Hello this is our jenkinsfile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Here you would put commands to test your project
            }
        }
        
        stage('Deploy to test') {
            steps {
                echo 'Deploying to test...'
                // Here you would put commands to deploy your project
            }
        }
        stage('Manual Approval') {
            steps {
                script {
                    // Pause pipeline and wait for user input
                    input message: 'Do you want to proceed?', ok: 'Proceed'
                }
            }
        }
        stage('Deploy to prod') {
            steps {
                echo 'Deploying to prod...'
                // Here you would put commands to test your project
            }
        }
    }
}
