pipeline {
    agent {
        node {
            label 'linux && java17'
        }
    }

    stages {
        stage('build') {
            steps {
                echo 'Hello Build'
            }
        }
        stage('test') {
            steps {
                echo 'Hello Test'
            }
        }
        stage('deploy') {
            steps {
                echo 'Hello Deploy'
            }
        }
    }

    post {
        always {
            echo "I will always say Hello again!"
        }
        success {
            echo "Yay, success"
        }
        failure {
            echo "Oh no, failure"
        }
        cleanup {
            echo "Don't care success or error"
        }
    }
}
