pipeline{
    agent any
    options {
        buildDiscarder(logRotator(numKeepstr: '5'))
    }
    stages {
        stage('docker build'){
            steps {
                sh 'docker -v'
                sh 'docker ps'
                sh 'whoami'
            }
        }
    }
    post {
        always {
            sh 'echo "This will always run"'
        }
    }
}