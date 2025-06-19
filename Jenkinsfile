pipeline{
    agent any
    environment {
        DEPLOY_TO = 'server'
    }
    stages {
        parrallel {
        stage('prodep') {
            when {
                environment name: 'DEPLOY_TO', value: 'server'
            }
            steps {
                echo "deploying to server"
                sleep 15
            }
        }
        stage('Build') {
            steps {
                echo "****building the application****"
                sleep 15
            }
        }
        stage('Testing') {
            steps {
                echo "****testing the application****"
                sleep 15
            }
        }
        stage('Docker') {
            steps {
                echo "****dockerizing the application****"
                sleep 15
            }
        }
        stage('Deploy') {
            when {
                branch 'release/*'
            }
            steps {
                echo "****deploying the application****"
                sleep 15
            }
        }
        stage('release') {
            when {
                tag pattern: "v*", comparator: "REGEXP"
            }
            steps {
                echo "****releasing the application****"
                sleep 15
            }
        }
    }
}
} 
