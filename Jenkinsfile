pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t rkalluru/d77-frontend .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push rkalluru/d77-frontend'
      }
    }

  }
}

