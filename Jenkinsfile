pipeline {
    agent any

    stages {
        stage('Inspect workspace') {
            steps {
                sh '''
                  echo "Current directory:"
                  pwd

                  echo "Files here:"
                  ls -la
                '''
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