pipeline {
agent any

    tools {
        maven 'Default'
        jdk 'JDK11'
        git 'Default'
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
