pipeline{
    agent any

    stages{
        stage('Build') {
            steps {
                echo "****bulding the application****"
           }

           stage('testing'){
            steps {
                echo "****testing the application****"
           }
           stage("Docker"){
            steps{
                echo "****dockerizing the application****"
            }

           }
        }
        }
    }
}
