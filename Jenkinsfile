pipeline {
    agent any

    tools {
        maven "Maven 3.x"  // Use the Maven tool configured in Jenkins
    }

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/Bnaik1982/Basic-Maven-Build-Pipeline.git'  // Replace with your repository URL
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}
