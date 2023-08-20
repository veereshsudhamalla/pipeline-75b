pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('test') {
      steps {
        echo 'i want to test'
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            echo 'i want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'i want to operate'
          }
        }

      }
    }

  }
}