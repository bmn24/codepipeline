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
        git (url: 'https://github.com/bmn24/codepipeline.git',
        credentialsId: 'git_hub',
        branch: 'master',) 
      }
    }
  }
}
