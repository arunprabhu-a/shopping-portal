pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the build job'
        sh 'npm install'
        sleep 4
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
        sleep 9
      }
    }

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
        sleep 7
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'This is my first pipeline as code...'
    }

  }
}