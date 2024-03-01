pipeline{
    agent any
    environment {
        TEST_1 = "test_env no .1"
        TEST_2 = "test_env no .2"
        TEST_3 = "test_env no .3"
        
    }
        stages {
            stage('build') {
               steps {
                sh '''
                echo $TEST -------$TEST_1
                sleep 5 ; ls'
               '''
               }
            }
            stage('build_11') {
               steps {
                sh '''
                echo $TEST_2 -------$TEST_3
                 sleep 10 '
               '''
               }
            }
             stage('test') {  
               steps {
                
                sh '''
                 echo $TEST_1 -------$TEST_2
                 sleep 10
                 '''
               }
                   
              
            }   
        
            
        }
}