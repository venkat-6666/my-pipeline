pipeline {
    agent any
    environment {
        a = '11'
    }
    stages {
        stage('condition') {
            when {
                expression { return env.a == '10' }
            }
            steps {
                echo "Condition is true"
            }
        }
    }
}
