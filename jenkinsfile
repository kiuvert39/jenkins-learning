pipeline {
    agent any

    stages {
        stage("checkout") {
            steps {
                echo 'Checking out code...'
            }
        }

        stage("Run script") {
            steps {
                sh "echo Hello from Jenkins"
            }
        }
    }

}