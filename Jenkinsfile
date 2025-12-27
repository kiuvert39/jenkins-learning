pipeline {
    agent any

    stages {

        stage('build') {
            steps {
                echo 'Building the project...'
            }
        }

        stage('test') {
            steps {
                sh '''
                    echo 'Running tests...'
                    exit 1
                ''' 
            }
        }

        stage('deploy') {
            steps {
                echo 'Deploying the project...'
            }
        }
    }

}