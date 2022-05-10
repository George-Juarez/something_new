pipeline {
  agent any
  triggers {
   cron('H/15 * * * *')
  }
  stages {
    stage('echo') {
      steps {
        echo 'hello from the trigger'
      }
    }
    stage('yelp'){
      steps{
        echo 'leaving yelp reviews helps'
      }
    }
  }
}
