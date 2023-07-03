pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                    return env.CHANGE_BRANCH == 'main' && env.CHANGE_TARGET == 'merge'
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
            }
        }
    }
}
