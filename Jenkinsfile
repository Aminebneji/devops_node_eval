pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker-compose build'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo 'Application déployée et en cours d\'exécution'
                }
            }
        }
    }

    post {
        always {
            sh 'docker-compose down'
        }
    }
}
