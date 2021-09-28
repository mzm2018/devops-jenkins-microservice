pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'}}
	enviornment {
		maven = tool 'maven'
		PATH = "maven:$PATH"
	}


	stages {
		stage('Build') {
			steps {
				echo 'build;'
				sh 'mvn --version'
			}
		}
			stage('Test') {
			steps {
				echo "Test"
			}
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
