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
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}
