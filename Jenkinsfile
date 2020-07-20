pipeline {
    agent any
    environment{
        PATH="/opt/maven3/bin:$PATH"
    }
    stages{
        stage('This is my Java project'){
            parallel{
        stage('Cleaning dir') {
            steps {
                sh "rm -rf Test-Dev"
            }
        }
        stage('git checkout') {
            steps {
               git 'https://github.com/mohantyprasannajit/Test-Dev.git'
               
            }
        }
        stage('MVN BUILD') {
            steps {
        sh "mvn clean package"
            }
        }
        stage('Agent Test') {
            steps {
               echo "Agent are working"
               
            }
        }
    }
        }
    }
}
