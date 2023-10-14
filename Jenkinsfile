pipeline {
   agent { docker { image 'mcr.microsoft.com/playwright' 
    args '-e HOME=/tmp -e NPM_CONFIG_PREFIX=/tmp/.npm'} }
   stages {
      stage('e2e-tests') {
         steps {
            sh 'npm run upload:check'
         }
      }
   }
}