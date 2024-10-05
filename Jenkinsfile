pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withEnv(["PATH+NODEJS=/usr/local/bin:/usr/local/sbin"]) {
                                sh 'node -v'
                                sh 'npm install'
                    }
            }
        }
    }
}