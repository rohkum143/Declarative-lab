pipeline {
	 agent { docker{ image 'maven:3.3.3'}}
	 environment { 
		DISABLE_AUTH = 'true'
                DB_ENGINE    = 'sqlite'
         } 
	 stages{
           stage('build'){
	       environment { 
                AN_ACCESS_KEY = credentials('rohtash_id') 
            }
	       steps{
	        sh 'mvn --version'
		sh 'printenv'
		checkout scm
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
