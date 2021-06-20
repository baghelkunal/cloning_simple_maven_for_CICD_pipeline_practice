# cloning_simple_maven_for_CICD_pipeline_practice

java -jar target/gs-maven-0.1.0.jar

pipeline {
	agent any

	stages {
    	stage('Code') {
        	steps {
            	echo 'Hello World from Code0'
            	echo 'Hello World from Code1'
            	echo 'Hello World from Code2'
        	}
    	}
    	stage('Build') {
        	steps {
            	echo 'Hello World from Build Stage'
        	}
    	}
    	stage('Test') {
        	steps {
            	echo 'Hello World from Testing'
        	}
    	}
    	stage('Deploy') {
        	steps {
            	echo 'Hello World from Deployment'
        	}
    	}
	}
}
