pipeline{
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages{
    stage(mvn clean){
        steps{
            mvn clean
        }
    }
    stage('mvn install'){
        steps{
            mvn install
        }
    }
    stage('mvn package'){
        steps{
            mvn package
        }
    }

    }
}