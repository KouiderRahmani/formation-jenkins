pipeline{
    agent {
        docker{
            image:'22-alpine3.19'
        }
    }
    stages {
        stage('build') {
            steps{
                 sh 'build'  
            }
        }
    }
   
}