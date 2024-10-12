pipeline{
    agent {
        docker { image 'node:20.18.0-alpine3.20' }
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