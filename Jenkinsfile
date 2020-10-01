pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        git 'https://github.com/lerndevops/samplejavaapp.git'
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
