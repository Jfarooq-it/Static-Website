pipeline {
  agent any
  stages  {
    stage('Upload to AWS') {
      steps  {
         withAWS(region:’us-east-2’,credentials:’blueocean’) {
           s3Upload(file:’index.html’, bucket:’udacity-jenkins-project’)
      }
    }
  }
}

