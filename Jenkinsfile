pipeline{
    agent any
    parameters{
        string(name: 'PARAM_String', defaultValue: 'this the parameter value', descrption:'display the parameter')

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
             
                
               
               
                   
              
               
        
            
        }
}