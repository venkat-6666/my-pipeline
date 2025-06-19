pipeline{
    agent any
    stages{
        stage('prodep'){
            when {
                expression {BRANCH_NAME ==~ /(producation|staging)/}
            }
            steps{
                echo "deploying to production or staging"
            }
        }

    }
 }
