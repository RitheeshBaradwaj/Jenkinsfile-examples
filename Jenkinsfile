pipeline {
    agent any
    stages {
        stage('Build Stage') {
            steps {
                echo "We are at Building..."
                echo "Building finished!"
            }
        }
        stage('Testing Stage') {
            steps {
                echo "Testing..."
                echo "Testing finished!"
            }
        }
        stage('Deployment Stage') {
            steps {
                echo "Deploying..."
                echo "Deploying finished"
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
