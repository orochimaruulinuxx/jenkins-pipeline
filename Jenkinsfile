pipeline{
    agent any
    stages{
    stage(hello){
        steps{
            sh 'echo hello'
        }
    }
    stage('clean articfat'){
        steps{
            sh 'mvn clean'
        }
    }

    }
}