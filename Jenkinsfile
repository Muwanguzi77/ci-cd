pipeline {
    //agent { docker { image 'php:8.4.8-alpine3.22' } }
    agent {
  docker {
    image 'php:8.4.8-windowsservercore'  // Windows container
    args '-v C:\\ProgramData\\Jenkins\\workspace:C:\\workspace'  // Windows volume mount
          }
            }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
            }
        }
    }
}
