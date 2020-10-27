pipeline {
  agent any
  stages {
    stage('getcode') {
      steps {
        git(url: 'https://github.com/saikishore789/my-app.git', branch: 'master', changelog: true, poll: true)
      }
    }

    stage('maven') {
      steps {
        sh 'mvn package'
      }
    }

  }
}