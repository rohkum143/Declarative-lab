pipeline {
     agent none
      stages {
        stage ('build') {
        agent any
         steps { 
           sh 'mvn --version'
              
              
           }
        }
        stage ('Example Test')  {
        agent any
         steps {
           sh 'java -version'
         }
       }
      }
    }
