pipeline{
    agent any
    parameters{
        string(name: 'PARAM_String', defaultValue: 'input_param', description:'this is the value of param')
        text(name: 'DEPLOY_TEXT', defaultValue: 'One\nTwo\nThree\n', description: 'this is the text value') 
        booleanParam(name: 'TOOGLE', defaultValue: true, description: 'true or false') 
    }
        
        stages {
            stage('build') {
               steps {
                sh '''
                echo $PARAM_String
                sleep 5 ; ls
               '''
               }
            }
            stage('build_11') {
               steps {
                script {
                    echo "${params.PARAM_String}"
                }
               }
            }
    
            
        }
}