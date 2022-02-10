pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                git checkout develop
                git checkout -b params.tipoBranch+"/"+params.nomeBranch
            }
        }
    }
}
