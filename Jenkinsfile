pipeline {
    agent any
    stages {
      stage(‘Upload’) {
        steps {
          withAWS(region:’us-east-2’,credentials:’UJP’) {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:’udacity-jenkins-project’)
          }
        }
      }
    }
}
