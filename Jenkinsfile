pipeline {
    agent any
    stages {
        stage('build') {
            steps {
               sh './gradlew build --no-daemon' 
            }
        }
    }
  post {
    always {
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
