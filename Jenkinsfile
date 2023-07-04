pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                    return env.GIT_BRANCH == 'origin/main' && env.CHANGE_TARGET == 'merge'
                }
            }
            steps {
                // Perform build steps here
                sh 'echo "Building..."'
            }
        }

        stage('Deploy') {
            steps {
                // Perform deployment steps here
                sh 'echo "Deploying..."'
                sh 'env'
            }
        }
    }
}
