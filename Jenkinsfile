pipeline{
    agent any
    parameters{
         string(name: 'PARAM_String', defaultValue: 'input_param', description:'this is the value of param')
         text(name: 'BIOGRAPHY', defaultValue: 'Please enter some thins', description: 'Enter some information about the person') 
         booleanParam(name: 'TOOGLE', defaultValue: true, description: 'true or false') 
          choice(name: 'CHOICE', choices: ['drinks', 'vegetables', 'fruits'], description: 'select something int he choice')
               }
        
        stages {
            stage('build') {
               steps {
                sh '''
                echo " PARAM_STRING :--   $PARAM_String "
                echo " bIOGRAPHY :--   $BIOGRAPHY "
                echo "tOOGLE :---     $TOOGLE"
                echo "cHOICE :--   $CHOICE"
                sleep 5 ; ls
               '''
               }
            }
            
            stage('build_11') {
               steps {
                script {
                    echo "  PARAM_STRING :-----   ${params.PARAM_String}"
                    echo "bIOGRAPHY :----     ${params.BIOGRAPHY}"
                    echo  "tOOGLE :--- ${params.TOOGLE}"
                    echo  "choice:-------     ${params.CHOICE}"
                    
                }
               }
            }
        }
            
        
}