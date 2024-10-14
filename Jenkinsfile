pipeline{
    agent any

    
    stages {
        stage('build') {
            steps{
               echo 'build !' 
            }
        }

        stage('deployement production ') {
            
            when{
                branch 'prod'
            }
            input{
                message 'Voulez-vous deployer en production ?'
                ok 'deployer !'
                submitter 'admin,devops'
                submitterParameter 'USER_SUBMIT'
                parameters {
                string (name : 'VERSION', defaultValue:'latest',description : 'une version ')
                }
            }
            steps{
               echo "user : ${USER_SUBMIT}"
               echo "version : ${VERSION}"
               echo "deploy !"
            }
        }
    }

   
}