pipeline {
  agent any
  stages {
stage('clone repo') {
          steps {
              sh("""
              git config --global credential.username VijayaLakshmiSaggam
              git config --global credential.helper "!echo password=Project20a; echo"
              git clone https://github.com/VijayaLakshmiSaggam/samplejavaapp.git
              echo "pulled the code"
              """)
          }

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

