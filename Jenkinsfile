pipeline {
     agent any
     stages {
       stage('Build') {
         Steps {
             sh 'echo "Hello World"'
             sh '''
                 echo "Multiline shell steps work too"
                 ls -lah
             '''
            }
       }
     }
}
  
