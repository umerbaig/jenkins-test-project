pipeline {
  agent any
  tools (nodejs "18.5.0")
  stages {
    stage('checkout from git') {
      parallel {
        stage('checkout from git') {
          steps {
            git(url: 'https://github.com/umerbaig/jenkins-test-project', branch: 'main')
          }
        }

        stage('log') {
          steps {
            sh '''git -v
node -v'''
          }
        }

      }
    }

    stage('npm install') {
      steps {
        sh 'npm install'
      }
    }

  }
}