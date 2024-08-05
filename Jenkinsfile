pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'To plan the app development'
      }
    }

    stage('Code') {
      steps {
        echo 'Developer develop the code'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'The code should be build'
          }
        }

        stage('Test') {
          steps {
            echo 'The code should be tested'
          }
        }

        stage('Deploy') {
          steps {
            echo 'The code should be deployed'
          }
        }

        stage('Operate') {
          steps {
            echo 'we can access the application'
          }
        }

      }
    }

  }
}