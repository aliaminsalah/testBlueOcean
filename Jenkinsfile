pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy is completted'
      }
    }

  }
}