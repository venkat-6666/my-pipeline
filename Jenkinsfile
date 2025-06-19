pipeline{
    agent any
    environment{
        DEPLOY_TO = 'server'
    }
    stages{
        stage('prodep'){
            when{
                environment name: 'DEPLOY_TO', value: 'server'
            }
            steps{
                echo "deploying to server"
            }
        }
    }
}
