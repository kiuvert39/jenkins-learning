pipeline {
    agent any

    stages {
        stage('Generate output') {
            steps {
                sh '''
                    pwd
                    ls -la
                    echo "Build completed at $(date)" > build.log
                    ls -la
                    '''
            }
        }
    }


    post {
        always {
            archiveArtifacts artifacts: 'build.log', fingerprint: true
        }
    }
}