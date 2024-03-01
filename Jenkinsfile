pipeline{
    agent any
    parameters{
        validatingString(name: 'PARAM_String', defaultValue: 'param', descrption:'display the parameter')

    }
        
        stages {
            stage('build') {
               steps {
                sh '''
                echo ${params.PARAM_String}
                sleep 5 ; ls
               '''
               }
            }
            stage('build_11') {
               steps {
                sh '''
                 sleep 10 
               '''
               }
            }
             stage('test') {  
               steps {
                script {

                }
                
               
               }
                   
              
            }   
        
            
        }
}