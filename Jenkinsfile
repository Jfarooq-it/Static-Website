pipeline {
  agent any
  stages  {           
       stage('Upload to AWS') 
    {
      steps {
          withAWS(region:’us-east-2’,credentials:’AKIA2OTEMD4Y5RSA4CNI’) {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:’udacity-jenkins-project’)
          }
     }
          }
}
