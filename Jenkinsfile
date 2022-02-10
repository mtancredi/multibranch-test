pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    git remote set-url develop https://mtancredi:emerasoft1@github.mtancredi.git
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"
                    
                '''
            }
        }
    }
}
