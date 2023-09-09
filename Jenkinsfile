pipeline{
    agent any
    stages{
    stage(mvn clean){
        steps{
            sh '/opt/maven/bin/mvn clean'
        }
    }
    stage('mvn install'){
        steps{
            sh '/opt/maven/bin/mvn install'
        }
    }
    stage('mvn package'){
        steps{
            sh '/opt/maven/bin/mvn package'
        }
    }

    }
}