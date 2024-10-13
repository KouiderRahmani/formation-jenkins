pipeline{
    agent any

    
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
                submitterParameter 'USER_SUBMIT'
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