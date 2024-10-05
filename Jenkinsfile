pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withEnv(["PATH+NODEJS=/usr/local/bin:/usr/local/sbin:/bin/sh"]) {
                             sh 'bash -c "node -v"'
                             sh 'bash -c "npm install"'
                    }
            }
        }
    }
}