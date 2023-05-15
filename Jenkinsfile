pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
//                 script {
//                     properties([pipelineTriggers([pollSCM('* * * * *')])])
//                 }
                git 'https://github.com/yzion10/TestProject.git'
            }
        }
        stage('run python')
        {
            steps {
                script
                {
                   bat 'C:\\DevOps\\GIT\\14.05.2023\\TestProject\\venv\\Scripts\\python.exe C:\\DevOps\\GIT\\14.05.2023\\TestProject\\second.py'
                }
            }
        }
    }
}
