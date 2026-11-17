
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/veerbasannaashwini2005/week.git'
            }
        }

        stage('Compile') {
            steps {
<<<<<<< HEAD
                bat 'javac HelloWorld.java'
=======
                sh 'javac HelloWorld.java'
>>>>>>> 5f2e80aed0da4fa197578be42c09283a088350eb
            }
        }

        stage('Run') {
            steps {
<<<<<<< HEAD
                bat 'java HelloWorld'
=======
                sh 'java HelloWorld'
>>>>>>> 5f2e80aed0da4fa197578be42c09283a088350eb
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
