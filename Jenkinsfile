pipeline {
	//agent any
	agent { docker { image 'maven:3.8.7'} }
	stages {
		stage('Build') {
			steps {
				echo 'mvn --version'
				echo "Build"
			}
		}
				stage('Test') {
			steps {
				echo "Test"
			}
		}
				stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
post {
	always {
		echo 'I am awesome. I run always'
	}
	success {
		echo 'I run when you are successfull'
	}
	failure {
		echo 'I run when you are fail'
		}
    }
}
