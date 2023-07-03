pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                    return env.BRANCH_NAME == 'main' && env.CHANGE_ID != null
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
