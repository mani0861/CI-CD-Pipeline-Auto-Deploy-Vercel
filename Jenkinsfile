pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/mani0861/CI-CD-Pipeline-Auto-Deploy-Vercel.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build Project') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Success') {
            steps {
                echo 'CI/CD Pipeline executed successfully 🚀'
            }
        }
    }
}
