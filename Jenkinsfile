pipeline {
  agent {
    node {
      label 'sampleSprintBoot'
    }

  }
  stages {
    stage('maven check') {
      parallel {
        stage('maven check') {
          steps {
            sh 'mvn clean'
            sh 'mvn clean package'
          }
        }
        stage('maven check 2') {
          steps {
            echo 'maven check 2'
          }
        }
        stage('maven check 3') {
          steps {
            echo 'check 3'
          }
        }
      }
    }
  }
}