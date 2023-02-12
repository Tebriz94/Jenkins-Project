pipeline {

	agent any
	environment {
		
		staging_server="54.90.1.38"
	}	


	stages {

		stage("Deploy to Remote Apache Server"){

			steps {

			sh 'scp -r ${WORKSPACE}/* ec2-user@${staging_server}:/var/www/html/'
		
	
		      }	

		}

	}

}
