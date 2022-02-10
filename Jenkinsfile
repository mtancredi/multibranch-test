pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git checkout develop
                    git checkout -b "${tipoBranch}"/"${nomeBranch}"
                    touch test.txt
                    git remote set-url origin https://mtancredi:+${password}@github.com/mtancredi/project.git
                    git add test.txt MyProject/src
                    git commit -m "test"
                    git push --set-upstream origin "${tipoBranch}"/"${nomeBranch}"

                '''
            }
        }
    }
}
