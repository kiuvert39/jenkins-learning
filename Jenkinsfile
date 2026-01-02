pipeline {
    agent any

    stages {
        stage('user secret safely'){
            steps {
                withCredentials([string(credentialsId: 'demo-secret', variable: 'MY_SECRET')]){
                    sh'''
                        echo "secret is masked"
                        echo "$MY_SECRET" > sercret.txt
                    '''

                }
            }
        }
    }


    post {
        always {
            archiveArtifacts artifacts: 'sercret.txt', fingerprint: true
        }
    }
}