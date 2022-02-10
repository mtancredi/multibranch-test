pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    touch test.txt
                    git init
                    git config user.name "someone"
                    git config user.email "someone@someplace.com"
                    pwd
                    git add text.txt MyProject/src
                    git commit -m "test"
                    git push
                '''
            }
        }
    }
}
