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
                    git init
                    git config user.name "someone"
                    git config user.email "someone@someplace.com"
                    git add *
                    git commit -m "test"
                    git push
                '''
            }
        }
    }
}
