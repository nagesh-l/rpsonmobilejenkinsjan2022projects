pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'blueocean_print'
        sh 'echo "build success"'
      }
    }

    stage('jtest') {
      parallel {
        stage('jtest') {
          steps {
            sleep 1
          }
        }

        stage('test_parallel') {
          steps {
            sleep 1
          }
        }

      }
    }

  }
}