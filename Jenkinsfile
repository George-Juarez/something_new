pipeline {
  agent any
  stages {
    stage('echo') {
      parallel {
        stage('echo') {
          steps {
            echo 'hello from the trigger'
          }
        }

        stage('') {
          steps {
            echo 'yoyo'
          }
        }

      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}