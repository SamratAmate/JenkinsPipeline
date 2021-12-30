pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
                sh 'pwd'
            }
        }
        stage('Docker Build') {
            steps {
                sh '''
                docker images -a'''
            }
        }
    }
}
