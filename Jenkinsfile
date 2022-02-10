pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    git remote set-url origin https://mtancredi:emerasoft1@github.mtancredi.git
                '''
            }
        }
    }
}
