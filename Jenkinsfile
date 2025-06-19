pipeline{
    agent any
    environment {
        DEPLOY_TO = 'server'
    }
    stages {
        stage('prodep') {
            when {
                environment name: 'DEPLOY_TO', value: 'server'
            }
            steps {
                echo "deploying to server"
            }
        }
        stage('Build') {
            steps {
                echo "****building the application****"
            }
        }
        stage('Testing') {
            steps {
                echo "****testing the application****"
            }
        }
        stage('Docker') {
            steps {
                echo "****dockerizing the application****"
            }
        }
        stage('Deploy') {
            steps {
                echo "****deploying the application****"
            }
        }
        stage('release') {
            steps {
                echo "****releasing the application****"
            }
        }
    }
}
