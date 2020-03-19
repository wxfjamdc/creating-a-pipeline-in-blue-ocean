pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''sh \'npm config set registry https://registry.npm.taobao.org --global\'
sh \'npm config set disturl https://npm.taobao.org/dist --global\'
npm install'''
      }
    }

  }
}