pipeline{
    agent any
    stages{
    stage(mvn clean){
        steps{
            sh 'mvn clean'
        }
    }
    stage('mvn install'){
        steps{
            sh 'mvn install'
        }
    }

    }
}