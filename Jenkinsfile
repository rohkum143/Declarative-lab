pipeline {
	 agent any
	   stages{
            stage('build'){
	       steps{
	        sh 'echo "hellow world" '
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
