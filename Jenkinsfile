pipeline {
    agent any

    stages {
        stage('CREDS') {
            steps {
               // This is accessing credential of type username and password
               withCredentials([usernamePassword(credentialsId: 'test_up', usernameVariable: 'USER_NAME', passwordVariable: 'PASS')]) {
                    echo "$USER_NAME $PASS"
                    sh '''
                        echo "$USER_NAME $PASS"
                    '''
               }

                
            }
        }
    }
}