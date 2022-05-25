pipeline {
    agent any
    environment {
        PATH = "D:\softwares\maven"
    }
    stages {
        stage("clone code"){
            steps{
                url:'https://github.com/Hssanjay/jenkinsjob.git'
            }
        }
        stage ("build code"){
            steps{
                sh "mvn clean install"
            }
        }
