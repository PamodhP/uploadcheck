pipeline {
   agent { docker { image 'mcr.microsoft.com/playwright' 
   stages {
      stage('e2e-tests') {
         steps {
            sh 'npm run upload:check'
         }
      }
   }
}