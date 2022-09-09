pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testing'
          }
        }

        stage('parallel') {
          steps {
            echo 'running'
          }
        }

      }
    }

    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'Clean'
      }
    }

  }
}