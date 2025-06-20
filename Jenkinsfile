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
            //this will run after the pipeline is scuccessful completed
            scuccess{
                echo "********====Pipeline is successful======*********"
            }
            //this will run after the pipeline is failed
            failure {
                echo "********====Pipeline is failed======*********"
            }
            //this will run after the pipeline is successful or failed
            always {
                echo "********====Pipeline is completed======*********"
            }
        }
}
