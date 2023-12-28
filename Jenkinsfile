pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build'
            }
        }

        stage('Test') {
            steps {
                echo 'Test'
                sh('error')
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }

    post {
        always {
            echo 'I will always say Hello again!'
        }

        success {
            echo 'Yah, success!'
        }

        failure {
            echo 'Oh no, failure!'
        }

        cleanup {
            echo "Don't care success or error"
        }
    }
}