pipeline {
    agent any
    stages {
        stage('Build Stage') {
            steps {
                sh 'echo "We are at Building..."'
                sh 'echo "Building finished!"'
            }
        }
        stage('Testing Stage') {
            steps {
                sh 'echo "Testing..."'
                sh 'echo "Testing finished!"'
            }
        }
        stage('Deployment Stage') {
            steps {
                sh 'echo "Deploying..."'
                sh 'echo "Deploying finished"'
            }
        }
        
    }
    post {
        always {
            echo 'We came to an end!'
        }
        success {
            echo 'Build is Successful brother!'
        }
        failure {
            echo 'Sorry mate! Build is Failed! :('
        }
        unstable {
            echo 'Run was marked as unstable'
        }
        changed {
            echo 'Hey look at this, Pipeline state is changed.'
        }
    }
}
