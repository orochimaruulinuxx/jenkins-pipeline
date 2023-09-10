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
        nexusArtifactUploader artifacts: [[artifactId: 'bioMedical',
         classifier: '', file: 'target/bioMedical-0.0.3-SNAPSHOT.jar',
          type: 'jar']], credentialsId: 'NexusID', groupId: 'com.spring',
          nexusUrl: 'ec2-18-204-9-87.compute-1.amazonaws.com:8081', 
          nexusVersion: 'nexus3', protocol: 'http',
           repository: 'project-app1', version: '0.0.3-SNAPSHOT'
        }

    }

    }
}