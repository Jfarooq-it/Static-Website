pipeline {
  agent any
  stages  {
    stage('Upload to AWS'), 
    withAWS(region:'us-east-2') {
      steps  {
          sh 'echo "Hello World"'
          sh '''
                echo "Multiline shell steps works too"
                ls -lah
             '''
      }
    }
  }
}

