pipeline {
    agent any

    stages {
        stage('git') {
            steps {
              git 'https://github.com/Deepthisambangi/Docker24jan.git'
            }
        }
        stage('Execute_java') {
            steps {
               sh '''git branch java
                     javac Hello.java
                     java Hello'''
            }
        }
        stage('execute_shell') {
            steps {
               sh '''git branch shell
                     ./fact.sh'''
            }
        }
        
    }
     
