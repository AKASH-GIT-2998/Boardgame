pipeline {
    agent {label 'slave_machine'}
    
    tools{
        jdk 'jdk11'
        maven 'maven3'
    }

    stages {
       
        stage('Compile') {
            steps {
                sh "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
