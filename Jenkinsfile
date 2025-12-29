pipeline {
    agent any

    stages {
        stage('Generate output') {
            steps {
                sh '''
                echo "Build completed at $(date)" > build.log
                echo "Build completed at $(date)"
                cat build.log
                '''
            }
        }
    }


    post {
        always {
            archiveArtifacts artifacts: 'build.log'
        }
    }
}