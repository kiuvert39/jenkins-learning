pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deploying to production'
            }
        }
    }

    // post {
    //     success {
    //         echo 'Build succeeded 🎉'
    //     }

    //        failure {
    //         echo 'Build failed ❌'
    //     }
    //     always {
    //         echo 'Pipeline finished (cleanup here)'
    //     }
    // }
}