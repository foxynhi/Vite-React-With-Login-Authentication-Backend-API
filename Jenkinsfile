pipeline {
    agent any


        stage('Start App') {
            steps {
                echo 'Starting app...'
                sh '''
                    ls -la
                    npm ci
                    vite
                '''
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished.'
        }
    }
}
