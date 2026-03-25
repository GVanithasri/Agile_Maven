pipeline {
    agent any

    environment {
        JAVA_HOME = "C:\\Program Files\\Java\\jdk-21"
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }

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
