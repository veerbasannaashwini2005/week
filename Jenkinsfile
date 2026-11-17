pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch:'main',
                url"https://github.com/veerbasannaashwini2005/week.git"

            }
        }
        stage('Build'){
            steps{
                echo'Building application';
            }
        }
        stage('Test'){
            steps{
                echo'Testing application';
            }
        }
        stage('Deploy'){
            steps{
                echo'Deploying application';
            }
        }
        post{
            success{
                echo'Pipeline completed successfully';
            }
            failure{
                echo'Pipeline failed';
            }
        }

    }
}