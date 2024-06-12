pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/its-abhishek/PES2UG21CS020_JENKINS', credentialsId: 'pes2ug21cs020'
            }
        }

        stage('Run Python Script') {
            steps {
                bat 'python test.py'
            }
        }
    }
}