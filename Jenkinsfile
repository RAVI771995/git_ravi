pipeline{
    agent any
    parameters{
         string(name: 'PARAM_String', defaultValue: 'input_param', description:'this is the value of param')
         text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person') 
         booleanParam(name: 'TOOGLE', defaultValue: true, description: 'true or false') 
    }
        
        stages {
            stage('build') {
               steps {
                sh '''
                echo $PARAM_String
                echo $BIOGRAPHY
                sleep 5 ; ls
               '''
               }
            }
            stage('build_11') {
               steps {
                script {
                    echo "${params.PARAM_String}"
                    echo "${params.BIOGRAPHY}"
                    
                }
               }
            }
    
            
        }
}