pipeline {
	 agent { docker{ image 'maven:3.3.3'}}
	 environment { 
		DISABLE_AUTH = 'true'
                DB_ENGINE    = 'sqlite'
         } 
	 stages{
           environment {
		  docker-pass = credentials('rohtash_ID')
	       }
	   stage('build'){
	       steps{
	        sh 'mvn --version'
		sh 'printenv'
	       }
	    } 	   
	 }
	 post {
	    always {
	       echo 'this will always run '
	    }
	    success {
	       echo 'this will run on sucessfull '
	       }
	     failure {
	        echo 'this will run on failure'
	     }
	 }
} 
