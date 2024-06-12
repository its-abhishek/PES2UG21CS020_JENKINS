pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/PES2UG21CS020_JENKINS/my-repo.git'
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python test.py'
                // Or use 'python script.py' if Python 3 is the default Python interpreter
            }
        }
    }
}
