pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withEnv(["PATH+NODEJS=/usr/local/bin:/usr/local/sbin:/bin/sh"]) {
                             bash -c "node -v"
                             bash -c "npm install"
                    }
            }
        }
    }
}