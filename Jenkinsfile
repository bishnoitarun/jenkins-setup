pipeline {
  agent any
  environment {
    GITHUB_CREDS = credentials('github-token')
  }
  stages {
    stage('Clone Repo') {
      steps {
        git credentialsId: "${GITHUB_CREDS}", url: 'https://github.com/bishnoitarun/jenkins-setup.git'
      }
    }
  }
}
