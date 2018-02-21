pipeline {
  agent any
  stages {
    stage('Scm') {
      steps {
        echo 'scm'
      }
    }
    stage('Build') {
      steps {
        echo 'build'
      }
    }
    stage("Test & Quality"){
      parallel {
      stage('Test') {
      steps {
        echo 'test'
      }
    }
    stage('Quality') {
      steps {
        echo 'build'
      }
    }
      }
    }
    
    stage('Dockerize') {
      steps {
        echo 'dockerize'
      }
    }
    stage('Publish Image') {
      steps {
        echo 'dockerize'
      }
    }

    stage('Deploy site') {
      steps {
        echo 'deploy'
      }
    }
  }
}