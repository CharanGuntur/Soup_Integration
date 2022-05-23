pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('batchscript') {
          steps{
          bat '''testrunner.bat "c:\\my projects\\my-project.xml" '''
            }
       }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    
}
