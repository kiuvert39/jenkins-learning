pipeline {
    agent any

    stages {
        stage('inspect workspace'){
            sh '''
                echo "current directory:"
                pwd
                echo "list files:"
                ls -la
            
            '''
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