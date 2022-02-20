pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'node --version'
        sh 'npm install --cache npm_cache'
        sh 'npm run build'
      }
    }

  }
}