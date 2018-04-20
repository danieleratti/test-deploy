pipeline {
  agent any
  stages {
    stage('prova') {
      parallel {
        stage('prova') {
          steps {
            mail(subject: 'Prova', body: 'Prova Deploy!!', to: 'danieleratti1992@gmail.com')
          }
        }
        stage('') {
          steps {
            sh 'echo "ciao" > "ciao.txt"'
            archiveArtifacts(artifacts: '*', allowEmptyArchive: true)
          }
        }
      }
    }
  }
}