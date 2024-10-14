pipeline{
    agent any
    tools{
        gradle 'gradle_8.11'
    }
    stages{
        stage('build'){
            steps{
                sh 'gradel -v'
            }
        }
    }
}
