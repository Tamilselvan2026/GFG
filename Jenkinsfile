
pipeline {
    agent {
        label 'linux-agent'
    }

    stages {
        stage('Welcome') {
            steps {
                echo 'Welcome to Jenkins Pipeline!'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building the application'
                sh 'hostname'
                sh 'whoami'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running application tests'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploying application'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed'
        }
        success {
            echo 'Pipeline SUCCESS!'
        }
        failure {
            echo 'Pipeline FAILED!'
        }
    }
}
