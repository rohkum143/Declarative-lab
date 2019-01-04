@Library('sharedlib@master') _
pipeline {
     agent none
      stages {
        stage ('build') {
        agent {docker 'maven:3-alpine'}
         steps { 
           sh 'mvn --version'
           runtest()
           }
        }
        stage ('Example Test')  {
        agent {docker 'openjdk:8-jre'}
         steps {
           sh 'java -version'
         }
       }
      }
    }
