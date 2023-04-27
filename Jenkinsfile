pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this is the Build job'
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        echo 'this is the test job'
        sh 'npm step'
      }
    }

    stage('Package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
    }

    stage('Archive') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'Shhoping Portal pipeline finished..'
    }

  }
}