pipeline {
  agent any
  stages {
    stage('asdf') {
      parallel {
        stage('asdf') {
          steps {
            load 'master/src/Cron%20Jobs/CronScript.groovy'
          }
        }

        stage('Hello') {
          steps {
            sh '''echo "Hello"
'''
          }
        }

      }
    }

  }
}