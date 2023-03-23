//scripted approach
/* node {
		echo "Build"
		echo "Test"
		echo "Integration Test"
  } */

//declarative approach 

pipeline {
	  agent any
	//agent { docker { image 'maven:3.6.3'} }
	//agent { docker { image 'node:alpine3.16'}}
	stages {
		stage("Build") {
		steps {
			//sh "mvn --version"
			//sh 'node --version'
			echo "Build"
			echo "$PATH"
			echo "BUILD_NUMBER - $env.BUILD_NUMBER"
			echo "BUILD_ID - $env.BUILD_ID"
			echo "JOB_NAME - $env.JOB_NAME"
			echo "BUILD-TAG - $env.BUILD_TAG"
			echo "BUILD-URL - $env.BUILD_URL"
		}
			}
		stage("Test"){
		steps {
			echo "Test"
			}
			}
		stage("Integration test") {
		    steps {
			   echo "Integration test"
			}
		}
	} 
	
    post {
		always{
			echo "Im awesome. I run always"
		}
		success {
			echo " I run when you are successful"
		}
		failure {
			echo " I run when you fail"
		
		}
	}
}