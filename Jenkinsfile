pipeline {
    agent any

    stages {
        stage('Start App') {
            steps {
                echo 'Starting app...'
                dir('frontend') {
                    bat '''
                        dir
                        call npm ci
                        call npx vite
                    '''
                }
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished.'
        }
    }
}
