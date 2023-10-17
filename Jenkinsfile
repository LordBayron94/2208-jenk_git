properties([pipelineTriggers([cron('* * * * 7')])])
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git 'https://github.com/LordBayron94/2208-jenk_git.git'
                bat 'python test.py'
            }
        }
        stage('Bye') {
            steps {
                bat 'python test.py'
            }
        }
    }
}
