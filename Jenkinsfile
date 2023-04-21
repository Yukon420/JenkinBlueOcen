pipeline {
  agent {
    node {
      label 'name'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''date
pwd
ls -lrth
ps -ef 
'''
          }
        }

        stage('env') {
          agent any
          environment {
            name = 'Rahul'
            city = 'Pune'
          }
          steps {
            echo 'hello Jenkin'
          }
        }

        stage('new1') {
          steps {
            sh 'echo ""Hello pipeline script "'
          }
        }

      }
    }

  }
  environment {
    name = 'rahul'
    city = 'pune'
  }
}