pipeline{
    agent {
        docker {
            image:'node:22-alpine3.19'
        }
     }
    stages {
        stage('build'){
            steps{
                sh 'npm -v'
            }
        }
    }

    post{
        always{
           echo 'always' 
        }
        success{
            echo 'success'
        }
    }
    

}