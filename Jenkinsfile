pipeline {
    agent any
    stages {
      stage('Upload to AWS') {
        steps {
          withAWS(region:’us-east-2’,credentials:’UJP2’) {
		    s3Upload(file:'index.html', bucket:'udacity-jenkins-project') 
		   }
          }
        }
      }
    }
