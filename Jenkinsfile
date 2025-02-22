pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
		git branch: 'main', 
                    url: 'https://github.com/selenemgr/Lab2-devops.git'
            }
        }

        stage('Build') {
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
                echo "Deploying application..."
            }
        }
    }
}
