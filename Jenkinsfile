pipeline {
    agent any 

    stages {    
        stage('test') { 
            steps { 
                sh 'echo hello'
            }            
        }
        stage('test1') { 
            steps { 
                sh 'echo $TEST'
            }            
        }
        stage('test3') {
            if (env.BRANCH_NAME == 'master') {
                echo 'I only execute on the master branch'
            } else {
                echo 'I execute elsewhere'
            }                        
        }        
    }
}
