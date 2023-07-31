pipeline {
    agent any
    when {
        expression {
            def payload = readJSON file: 'payload.json'
            def action = payload.action
            return action == 'review_requested'
        }
    }
    stages {
        stage('Build') {
            steps {
                // Perform build steps here
                sh 'echo "Building..."'
                sh "env"
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
