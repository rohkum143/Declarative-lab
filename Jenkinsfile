pipeline {
     agent none
      stages {
        stage ('build') {
        agent any
         steps { 
           sh 'hostname -i'
              
              
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
