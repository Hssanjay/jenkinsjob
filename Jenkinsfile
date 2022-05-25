pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                cmd: 'mvn clean package'
                }
        }
     }
    post {
       always {
          junit(
        allowEmptyResults: true,
        testResults: '*/test-reports/.xml'
      )
      }
   } 
}
