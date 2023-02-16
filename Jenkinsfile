pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'make build pes2ug20cs388'
            }
        }

        stage('Test') {
            steps {
                sh 'make test pes2ug20cs388'
            }
        }

        stage('Deploy') {
            steps {
                sh 'make deploy pes2ug20cs388'
            }
        }
    }

    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
