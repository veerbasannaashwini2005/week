
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Getting source code from GitHub'
                git branch: 'main',
                    url: 'https://github.com/veerbasannaashwini2005/week.git'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling Java program'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java program'
                bat 'java HelloWorld'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}
