//SCRIPTED PIPELINE
/* node {
	 *//* stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
	stage('Integration Test'){
	    echo "Integration Test"
	}
	stage('Package'){
	    echo"Package"
	} *//*

	echo "Build"
	echo "Tests"
	echo "Integration Tests"
	//echo "Build Package"
} */
// Declarative PIPELINE

/*
pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo "Build"
            }
        }
        stage('Test 1'){
            steps{
                echo "Test 1 Running"
            }
        }
        stage('Integration Tests'){\
            steps{
                echo "Integration Test running"
            }
        }
        stage('Package the jar'){
            steps{
                echo "Package the jar running"
            }
        }
    }
    post{
        always {
            echo "I am running always"
        }
        success {
            echo "I am successfully completed the build"
        }
        failure {
            echo "Build Failed for some reason"
        }
    }
} */

pipeline{
    agent { docker {image "maven:3.6.3" }}
    stages{
        stage('Build'){
            steps{
                echo "Build"
            }
        }
        stage('Test 1'){
            steps{
                echo "Test 1 Running"
            }
        }
        stage('Integration Tests'){\
            steps{
                echo "Integration Test running"
            }
        }
        stage('Package the jar'){
            steps{
                echo "Package the jar running"
            }
        }
    }
    post{
        always {
            echo "I am running always"
        }
        success {
            echo "I am successfully completed the build"
        }
        failure {
            echo "Build Failed for some reason"
        }
    }
}