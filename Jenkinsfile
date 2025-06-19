pipeline{
    agent any
    environment{
        a=10
    }
    stages{
        when{
            condition a=10
        }
        stage('condition')
        steps{
            echo "Condition is true"
        }
    }
}
