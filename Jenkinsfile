pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/GVanithasri/Agile_Maven.git'
            }
        }

        stage('Build and Test') {
            steps {
                bat '"C:\\Program Files\\apache-maven-3.9.14\\bin\\mvn" clean test'
            }
        }
    }
}
