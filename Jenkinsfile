pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                git 'https://github.com/mtancredi/multibranch-test'
                git checkout develop
                git checkout -b "${tipoBranch}"+"/"+"${nomeBranch}"
            }
        }
    }
}
