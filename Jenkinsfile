pipeline{
    agent any
    tools{
        gradle 'gradle_8.11'
       
        nodejs 'nodeJs_v_22.9.0' 
    }
    stages{
        stage('build'){
            steps{
                sh 'gradle -v'
                sh 'node -v'
            }
        }
    }
    post{
            success{
                  emailext (to: 'rahmanikouider.1@gmail.com', body: 'test body' ,
                          subject: 'test jenkins mail')
            }
        }
    
}
