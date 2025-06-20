pipeline{
    agent any
    stages {
        stage('Build') {
            steps {
                sh "hostname -i"
            }
        } 
    }
     post {
            //This will run after the pipeline is successfully completed
            success {
                echo "********====Pipeline is successful======*********"
            }
            //This will run after the pipeline has failed
            failure {
                echo "********====Pipeline is failed======*********"
            }
            //This will run after the pipeline is successful or failed
            always {
                echo "********====Pipeline is completed======*********"
            }
        }
}
