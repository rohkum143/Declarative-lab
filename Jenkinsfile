pipeline {
     agent none
      stages {
        stage ('build') {
        agent {docker 'maven:3-alpine'}
         steps { 
           sh 'mvn --version'
           }
        }
        stage ('Example Test') {
        agent { dokcer 'openjdk:8-jre'}
         steps {
           sh 'java -version'
         }
       }
      }
    }
