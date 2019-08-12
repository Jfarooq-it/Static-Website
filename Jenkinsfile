pipeline {
    agent any
    stages {
      stage('Build') {
        steps {
          echo "Hellooooo!"
          }
		  }
      stage('Build') {
        steps {
          withAWS(endpointUrl:'http://udacity-jenkins-project.s3-website.us-east-2.amazonaws.com', credentials:'AKIA2OTEMD4Y5RSA4CNI') {
		    s3Upload(file:'index.html', bucket:'udacity-jenkins-project') 
		   }
          }
        }
      }
    }
