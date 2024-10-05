pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withEnv(["PATH+NODEJS=/usr/local/bin:/usr/local/sbin"]) {
                                'node -v'
                                'npm install'
                    }
            }
        }
    }
}