pipeline {
  agent any
  tools {nodejs "nodenv" }
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/jruels/nodejs-jenkins'
      }
    }
    stage('Build') {
       steps {
         sh 'npm install'
       }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}
