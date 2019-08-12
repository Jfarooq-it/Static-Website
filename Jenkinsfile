pipeline {
    agent any
    stages {
      stage('Build') {
        steps {
          echo "Hellooooo!"
          }
		  }
      stage('Upload to AWS') {
        steps {
          withAWS(endpointUrl:'http://udacity-jenkins-project.s3.amazonaws.com/', credentials:'UJP1') {
		    s3Upload(file:'index.html', bucket:'udacity-jenkins-project') 
		   }
          }
        }
      }
    }
