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
    stage('upload artifact'){
        steps{
        sh 'curl --upload-file target/bioMedical-0.0.3-SNAPSHOT.jar -u admin:admin -v http://ec2-18-204-9-87.compute-1.amazonaws.com:8081/repository/project-app1/'
        }

    }

    }
}