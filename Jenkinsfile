pipeline {
  agent none
  stages {
    stage('sync') {
      parallel {
        stage('sync') {
          steps {
            echo 'sync source'
          }
        }
        stage('sync2') {
          steps {
            echo 'sync2'
          }
        }
        stage('') {
          steps {
            sh 'echo "HI"'
          }
        }
      }
    }
    stage('build') {
      steps {
        echo 'building'
      }
    }
    stage('test') {
      steps {
        echo 'test'
      }
    }
  }
}