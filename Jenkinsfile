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
                sh '''mvn clean'''
              //  readFile 'https://github.com/CharanGuntur/Soup_Integration/blob/master/sample.xml'
            }
            //post {
             // always {
            //    archiveArtifacts 'target/surefire-reports/**/*.xml'
               // junit 'target/surefire-reports/**/*.xml'
           //     }
          //  }
     }
}
}
