pipeline {
    agent any
    stages{
        stage("Hello") {
            steps {
                export PATH=$PATH:/path/to/your/python/bin
                sh "robot mytest.robot"
            }
        }
    }
}