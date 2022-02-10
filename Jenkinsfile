pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                nuovoBranch = params.tipoBranch+"/"+params.nomeBranch
                echo $nuovoBranch

            }
        }
    }
}
