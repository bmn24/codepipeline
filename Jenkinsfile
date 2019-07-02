Pipeline {
  agent any
  stages {
    stage('Cleanup') {
      steps {
        deleteDir()
      }
    }
    stage ('SCM (github)') {
      steps {
        git (url: 'https://github.dxc.com/schitti2/harmodel.git',
        credentialsId: 'tokenpass',
        branch: 'master',) 
      }
    }
  }
}
