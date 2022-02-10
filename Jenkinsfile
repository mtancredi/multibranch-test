pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    git remote set-url origin https://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@github.com/mtancredi/multibranch-test.git
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"
                '''
            }
        }
    }
}
