pipeline{
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }
            stage('Testing') {
                steps {
                    echo "Testing the application..."
                }
            }
            stage('Docker') {
                steps {
                    echo "Dockerizing the application..."
                }
            }
            stage('Deploy') {
                input {
                    message "Do you want to deploy the application?"
                    ok "Yes, deploy it!"
                    submitter 'devsai'
                }
                steps {
                    echo "Deploying the application..."
                }
            }
            stage('Release') {
                steps {
                    echo "Releasing the application..."
                }
            }
        } 
    }
