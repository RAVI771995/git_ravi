pipeline{
    agent any
   
        stages {
            stage('build') {
              

               steps {
                sh ' sleep 5 '
               }

            }
             stage('test') {

               steps {
                sh '''
                #!/bin/bash
                 ls -lrt
                 sleep 10
                 '''

                
               }
            }
        }
}