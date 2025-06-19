pipeline{
    agent any
    environment{
        // Define the environment
        name = "venkat"
        course = "GCP"
    }
    stages{
        stage('Build'){
            environment{
                // Define the environment
                course = "2025"
            }
            steps{
                echo "Welcome ${name}"
                echo "your ${course}"
                echo "my branch ${env.BUILD_NUMBER}"
            }
        }
    }
}
