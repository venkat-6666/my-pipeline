pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {
        stage('Example'){
            steps{
                echo "Hello, ${PERSON}!"
                echo "Biography: ${BIOGRAPHY}"
                echo "Toggle is set to: ${TOGGLE}"
                echo "You chose: ${CHOICE}"
                echo "Password: ${PASSWORD}"
                // Note: Avoid printing sensitive information like passwords in logs
                // Instead, use a secure way to store and retrieve sensitive data
                
            }
        }
    }
}  
