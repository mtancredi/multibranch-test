pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    touch README.md
                    git add README.md
                    git commit
                    git push
                '''
            }
        }
    }
}
