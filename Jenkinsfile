pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
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