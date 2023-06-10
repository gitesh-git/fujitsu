pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/gitesh/Documents/extract-file/apache-maven-3.9.1/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/fujitsu.war gitesh@127.0.1.1:/home/gitesh/Documents/extract-file/apache-tomcat-9.0.73/webapps'
	}
}}}
