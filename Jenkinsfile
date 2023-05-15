pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                script {
                    properties([pipelineTriggers([pollSCM('* * * * *')])])
                }
                git 'https://github.com/yzion10/TestProject.git'
            }
        }
        stage('run python') {
            steps {
                script 
                {
                   bat 'second.py'
                }
            }
        }
    }
}
