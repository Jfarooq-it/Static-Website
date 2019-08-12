pipeline {
    agent any
    stages {
      stage(‘Upload to AWS’) {
        steps {
          withAWS(credentials:’UJP’) {
            s3Upload(file:’index.html’, bucket:’udacity-jenkins-project’)
          }
        }
      }
    }
}
