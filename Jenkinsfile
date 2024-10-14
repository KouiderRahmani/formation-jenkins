pipeline{
    agent any
    tools{
        gradel 'gradel_8.11'
    }
    stages{
        stage('build'){
            steps{
                sh 'gradel -v'
            }
        }
    }
}
