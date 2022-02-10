pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                sh '''
                    git 'https://github.com/mtancredi/multibranch-test'
                    git checkout develop
                    git checkout -b "${tipoBranch}"+"/"+"${nomeBranch}"
                '''
            }
        }
    }
}
