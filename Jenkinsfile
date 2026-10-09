pipeline {
    agent any

    stages {
        stage('checkout code') {
            steps {
                checkout scm
            }
        }
         stage('setup python') {
            steps {
                sh "pip install -r requirements.txt"
            }
        }
        stage('run python program') {
            steps {
                sh "python3 extract.py"
            }
        }
    }
}