pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    touch test.txt
                    git remote set-url origin https://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@github.com/mtancredi/multibranch-test.git
                    git add test.txt MyProject/src
                    git commit -m "test"
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"

                '''
            }
        }
    }
}
