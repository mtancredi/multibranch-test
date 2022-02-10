pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                newBranch = "${tipoBranch}"+"/"+"${nomeBranch}"
                echo $newBranch
            }
        }
    }
}
