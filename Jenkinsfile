pipeline {
    agent any
    environment {
        PATH = "D:/softwares/maven/bin:$PATH"
    }
    stages {
        stage("clone code"){
            steps{
               git url:'https://github.com/Hssanjay/jenkinsjob.git'
            }
        }
        stage ("build code"){
            steps{
                sh "mvn clean install"
            }
        }
