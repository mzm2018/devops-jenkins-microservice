pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'}}
	stages {
		stage('Build') {
			steps {
				//echo 'mvn --version'
				echo 'build'
				echo "$PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
		}
	} 
	post {
		always {
			echo 'Im awesome. I run always'
		}
		success {
			echo ' I run when you are successfull'
		}
		failure {
			echo 'I run when you fail'
		}
	}
	}
