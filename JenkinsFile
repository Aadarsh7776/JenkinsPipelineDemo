pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Aadarsh7776/JenkinsPipelineDemo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling Java Program...'
                bat 'javac HelloWorld.java'
            }
        }
        stage('Run') {
            steps {
                echo 'Running Java Program...'
                bat 'java HelloWorld'
            }
        }
        stage('Success') {
            steps {
                echo 'Pipeline executed successfully!'
            }
        }
    }
}
