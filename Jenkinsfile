// SCRIPTED


// DECLARATIVE

pipeline{
	agent any
	// agent{docker {image 'node:22-alpine3.19'}}
	stages{
		stage('Build'){
			steps{
				// sh 'mvn --version'
				// sh 'node --version'
				echo "Build"
				echo "path - $path"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"


			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}

	post{
		always{
			echo "Im awesome .I run always"
		}
		success{
			echo " I run when u r successful"
		}
		failure{
			echo "I run when u fail "
		}
	}
}
