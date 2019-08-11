pipeline {
  agent any
  stages  {           
       stage('Upload to AWS') 
    {
      steps {
          withAWS(region:’us-east-2’) {
            s3Upload(bucket:’udacity-jenkins-project’)
          }
     }
          }
}
