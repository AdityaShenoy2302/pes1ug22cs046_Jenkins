pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o output hello1.cpp' // Compile the C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './Aditya' // Run the compiled executable
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...' // Modify this step based on deployment needs
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
