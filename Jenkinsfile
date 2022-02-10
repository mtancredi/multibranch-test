pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    touch test.txt
                    git add test.txt MyProject/src
                    git commit -m "test"
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"

                '''
            }
        }
    }
}
