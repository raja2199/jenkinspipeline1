pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'plan code for pipeline'
      }
    }

    stage('code') {
      steps {
        echo 'code for pipelne'
      }
    }

    stage('Bulid') {
      steps {
        echo 'bulid code for pipeline'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test code for pipeline'
          }
        }

        stage('Release') {
          steps {
            echo 'release code for pipeline'
          }
        }

        stage('Deploy') {
          steps {
            echo 'deploy code for pipeline'
          }
        }

        stage('Operate') {
          steps {
            echo 'operate code for pipeline'
          }
        }

      }
    }

  }
}