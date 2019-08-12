pipeline {
    agent any
    stages {
      stage(‘Upload to AWS’) {
        steps {
          withAWS(credentials:’UJP’) {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:’udacity-jenkins-project’)
          }
        }
      }
    }
}
