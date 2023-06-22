pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'This is Development Stage'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is Testing Stage'
          }
        }

        stage('Build') {
          steps {
            echo 'This is Build Stage'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is Deploymnet Stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'This is Operate'
          }
        }

      }
    }

  }
}