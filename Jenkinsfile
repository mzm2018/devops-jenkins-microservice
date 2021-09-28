pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'}}
	environment {
		mavenHome = tool 'maven'
		PATH = "$mavenHome:$PATH"
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo 'build;'

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
