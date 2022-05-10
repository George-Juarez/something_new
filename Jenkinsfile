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
    stage('yelp'){
      steps{
        echo 'leaving yelp reviews helps'
      }
    }
  }
  triggers {
    cron('H/15 * * * *')
  }
}
