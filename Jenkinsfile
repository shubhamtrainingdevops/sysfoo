pipeline{
    agent any
    
    tools{
        maven 'Maven 3.6.3'

    }
    stages{

        stage('Build'){
            steps{
                sh 'mvm compile'
            }
        }

        stage('Unit Test'){
            steps{
                sh 'mvm clean test'
            }
        }

        stage('Package'){
            steps{
                sh 'mvm package -DskipTests'
            }
        }

    }
}