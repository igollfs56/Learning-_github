pipeline {
    agent any
    stages{
        stage("Hello") {
            steps {
                export PATH=$PATH:/opt/homebrew/bin/python3
                sh "robot mytest.robot"
            }
        }
    }
}