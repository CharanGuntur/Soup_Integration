pipeline {
agent any

    tools {
        maven 'maven3'
        jdk 'jdk8'
    }
    stages {
        stage('Test') {
            steps {
                sh ''' mvn clean test '''
            }
            post {
              always {
                archiveArtifacts 'target/surefire-reports/**/*.xml'
                junit 'target/surefire-reports/**/*.xml'
                }
            }
     }
}
}
