pipeline{
    agent any
    stages{
        stage('prodep'){
            when {
                anyOf
                expression {BRANCH_NAME ==~ /(producation|staging)/}
                branch '123'
            }
            steps{
                echo "deploying to production or staging"
            }
        }

    }
 }
