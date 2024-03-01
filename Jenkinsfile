pipeline{
    agent {
        label 'slave_2'
    }
   
        stages {
            stage('build') {
               steps {
                sh ' sleep 5 '
               }
            stage('build_11') {
               steps {
                sh ' sleep 15 '
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
              stage('test22') {
               steps {
                sh ' sleep 15 '
               }
            }
            }
        }
}