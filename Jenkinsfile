pipeline {
    agent any
    stages {
      stage('Lint HTML') {
        steps {
          sh 'tidy -q -e *.html'
          }
		  }
      stage('Upload to AWS') {
        steps {
          withAWS(credentials:'UJP1') {
		    s3Upload(file:'index.html', bucket:'udacity-jenkins-project') 
		   }
          }
        }
      }
    }
