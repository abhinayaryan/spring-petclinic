pipeline {
    agent {
        label 'master'
    } 
    tools{
        maven 'Maven'
        jdk 'Java'
    }
    stages {
        stage('validate') {
            steps {
                sh 'mvn validate' 
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile' 
            }
        }
        stage('test') {
            steps {
                sh 'mvn test' 
            }
        }
        stage('pacage') {
            steps {
                sh 'mvn package' 
            }
        }
    }
}