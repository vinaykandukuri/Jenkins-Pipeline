pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'To Plan the Application'
      }
    }

    stage('Code') {
      steps {
        echo 'Developers develop the code'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'The Code should be Built'
          }
        }

        stage('Test') {
          steps {
            echo 'The code should be Tested'
          }
        }

        stage('Deploy') {
          steps {
            echo 'The code should be deployed'
          }
        }

        stage('Operate') {
          steps {
            echo 'We can access the code'
          }
        }

      }
    }

  }
}