pipeline{
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages{
    stage('mvn clean'){
        steps{
        sh 'mvn clean'
        }
    }
    stage('mvn install'){
        steps{
        sh 'mvn install'
        }
    }
    stage('mvn package'){
        steps{
        sh  'mvn package'
        }
    }

    }
}