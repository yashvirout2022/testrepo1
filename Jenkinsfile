pipeline {
    agent any

    stages {
        stage('checkout code') {
            steps {
                checkout scm
            }
        }
        stage('run python program') {
            steps {
                sh "python extract.py"
            }
        }
    }
}