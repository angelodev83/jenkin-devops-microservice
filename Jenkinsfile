//scripted approach
/* node {
		echo "Build"
		echo "Test"
		echo "Integration Test"
  } */

//declarative approach 

pipeline {
	agent any
	stages {
		stage("Build") {
		steps {
			echo "Build"
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
}