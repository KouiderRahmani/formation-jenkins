pipeline{
    agent any

     triggers{
        pollSCM('* * * * *')
     }
    
    
    stages {
        stage('build') {
            steps{
               echo 'build !' 
            }
        }
    }
    stages {
        stage('deployement production ') {
            input{
                message 'Voulez-vous deployer en production ?'
                ok 'deployer !'
                submitter 'admin,devops'
                submitParameter 'USER_SUBMIT'
                parameters (name : 'VERSION', defaultValue:'latest',description : 'une version ')
            }
            steps{
               echo "user : ${USER_SUBM}"
               echo "version : ${VERSION}"
               echo "deploy !"
            }
        }
    }

   
}