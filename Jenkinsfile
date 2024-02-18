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
                      cal 2024
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
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Here you would put commands to deploy your project
            }
        }
    }
}
