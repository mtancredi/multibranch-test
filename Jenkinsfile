pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"
                '''
            }
        }
    }
}
