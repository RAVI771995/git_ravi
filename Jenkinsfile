pipeline{
    agent none
        stages {
            stage('build') {
                agent {
                     label 'slave_1'
                }
               steps {
                sh ' sleep 5 ; ls'
               }
            }
            stage('build_11') {
                agent {
                        label 'slave_2'
                       }
               steps {
                sh ' sleep 10 '
               }
            }
             stage('test') {
                agent {
                       label 'slave_1'
                 }
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