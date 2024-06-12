pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/its-abhishek/PES2UG21CS020_JENKINS'
            }
        }

        stage('Run Python Script') {
            steps {
                bat 'python test.py'
                // Or specify the full path to Python if necessary
                // bat '"C:\\Path\\To\\Python\\python.exe" script.py'
            }
        }
    }
}
