
pipeline {
    agent any

    stages {
        stage('CREDS') {
            steps {
                  // First credential (USERNAMe & Password)
                  // This is accessing credential of type username and password
                 withCredentials([usernamePassword(credentialsId: 'test_up', usernameVariable: 'USER_NAME', passwordVariable: 'PASS')]) {
                   echo "$USER_NAME $PASS"
                    sh '''
                        echo "$USER_NAME $PASS"
                    '''
                }
                // Second credential (SEcreete text)
                //This is accessing credential of type Secrete text 
                 
                    withCredentials([string(credentialsId: 'Secrete_text', variable:'secret_text')]) {
                        echo "$secret_text"
                        sh '''
                           echo "$secret_text"
                        '''
                    }
                 

                  //third credential (SECRETE file)
                  //This is accessing credential of type Secrete file 
                withCredentials([file(credentialsId: 'Secret_file', variable: 'File_path')]) {
                   echo "$File_path"
                    sh '''
                      echo "$File_path"
                    '''                  
                }

                
                 // Fourth Credeential (SSH UN & Private key)
                 //This is accessing credential of type SSH username & private key 
                withCredentials([sshUserPrivateKey(credentialsId: 'SSH_KEY', usernameVariable: 'USER', keyFileVariable: 'SSH_key')]) {
                   echo "$USER $SSH_key"
                    sh '''
                    echo "$USER  $SSH_key"
                     ''' 
                }
                sshgent (credentials :['SSH_PEM']) {

                    sh '''
                    ls -lrt 
                    echo "startedt the server"
                    '''
                }

               

                
            
            }
        }    
    }
}
