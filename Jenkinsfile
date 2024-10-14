pipeline{
    agent any
    
    parameters{
        booleanParam(name:'DEPLOY_TO',defaultValue:false, description:'production ?')
    }
    
    stages {
        stage('build') {
            steps{
               echo 'build !' 
            }
        }

        stage('deployement production ') {
            
            when{
                allOf{
                    branch 'main'
                    equals exepted:true ,actual:params.DEPLOY_TO
                }
            }
            
            steps{
               echo "deploy !"
            }
        }
    }

   
}