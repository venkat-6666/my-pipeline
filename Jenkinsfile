pipeline{
    agent any
    stages{
        stage('prodep'){
            when {
                branch '123'
                branch 'production'
            }
            steps{
                echo "deploying to production or staging"
            }
        }

    }
 }
