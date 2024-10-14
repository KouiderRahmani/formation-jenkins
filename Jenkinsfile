pipeline{
    agent any
    tools{
        gradle 'gradel_8.11'
    }
    stages{
        stage('build'){
            steps{
                sh 'gradel -v'
            }
        }
    }
}
