pipeline{
    agent {
        docker {
            image:'node:21-alpine'
        }
     }
    stages {
        stage('build'){
            steps{
                echo "BRANCH_NAME: ${env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY: ${env.BRANCH_IS_PRIMARY}"
                echo "CI: ${env.CI}"
                echo "BUILD_NUMBER:RANCHE_NAME: ${env.BUILD_NUMBER}"
                echo "JENKINS_URL: ${env.JENKINS_URL}"
                echo "MY_VAR: ${env.MY_VAR}"
                echo "MY_NUMBER: ${env.MY_NUMBER}"
                sh   'printenv'
                sh   'npm -v'
            }
        }
    }

    post{
        always{
           echo'always' 
        }
        success{
            echo'success'
        }
    }
    

}