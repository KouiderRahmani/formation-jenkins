pipeline{
    agent any

    stages {
        stage('build') {
            failFast true;
            parallel{
                stage('back end  ') {
                    
                    steps{
                    echo "back end  !"
                    }
                }
                stage('frent end  ') {
                    
                    steps{
                    echo "frent end  !"
                    }
                }
            }
        
        }
        stage('deployement production ') {
            
            steps{
                    echo "deploy !"
            }
        }
    }

}
