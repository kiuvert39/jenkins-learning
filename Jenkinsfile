pipeline {
    agent any

    stages {
        stage('user secret safely'){
            stpreps {
                withCredentials([string(credentialsId:'demo-scret', vaariable: 'My_SECRET')]) {
                    sh'''
                        echo "secret is masked"
                        echo "$My_SECRET" > sercret.txt
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