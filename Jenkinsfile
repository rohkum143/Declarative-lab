pipeline {
	 agent { docker{ image 'maven:3.3.3'}}
	 stages{
	   stage('build'){
	       steps{
	        sh 'mvn --version' 
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
