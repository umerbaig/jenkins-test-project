pipeline {
  agent any
  stages {
    stage('checkout from git') {
      steps {
        git(url: 'https://github.com/umerbaig/jenkins-test-project', branch: 'main')
      }
    }

  }
}