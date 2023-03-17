pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build step'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 3
      }
    }

  }
}