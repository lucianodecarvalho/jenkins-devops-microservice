//SCRIPTED
//DECLARATIVE
pipeline {
	//agent any
	environment {
		dockerHome = tool 'myDocker'
	}
//	agent { docker{ image 'maven:3.6.3'} }
	//agent { docker{ image 'node:13.8'} }

	stages {
		stage('Build'){
			steps {
				sh "node --version"
				echo "Build"
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps {
				echo "Integration Test"
			}
		}
	}
	
	post {
		always {
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are succesfull'
		}
		failure {
			echo 'I run when you are failures'
		}
	}
}
