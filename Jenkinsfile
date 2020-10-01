pipeline {
  agent any
  stages {
    stage('Clone sources') {
           git url: 'https://github.com/VijayaLakshmiSaggam/samplejavaapp'
                           }
    stage('Compile') {
      steps {
        sh script: 'mvn clean compile'
            }
                     }
    stage('Test') {
      steps {
        sh script: 'mvn test'
            }
                     }
    stage('Package') {
      steps {
        sh script: 'mvn package'
            }
                     }
         }
         }

