pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Coutinho125/23BBS0178-DevOps-Project.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Docker Build') {
            steps {
                script {
                    sh 'docker build -t subham/website:v1 .'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment step will be added later (Kubernetes)'
            }
        }
    }
}
