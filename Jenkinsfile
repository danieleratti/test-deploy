pipeline {
  agent any
  stages {
    stage('prova') {
      parallel {
        stage('prova') {
          steps {
            echo 'Hello World!'
          }
        }
        stage('Ciao') {
          steps {
            sh 'echo "ciao2" > "ciao2.txt"'
            archiveArtifacts(artifacts: '*', allowEmptyArchive: true)
          }
        }
      }
    }
  }
}