pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
                sh 'pwd'
            }
        stage('Docker Build') {
            steps {
powershell '''cd azure-vote/
docker images -a
docker build -t jenkins-pipeline .
docker images -a'''
            }
        }
    }
}
