pipeline {
    agent any

    //tools {
    //    nodejs 'NodeJS 22.9.0'  // Use the Node.js version configured in Jenkins
    //}

    stages {
        stage('Clone Repository') {
            steps {
                // Clone the GitHub repository
                git url: 'https://github.com/Sparticussheena/simple-node-js-react-npm-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install npm dependencies
                sh 'npm install'
            }
        }

        stage('Build Application') {
            steps {
                // Build the React application
                sh 'npm run build'
            }
        }

        stage('Run Tests') {
            steps {
                // Run any tests
                sh 'npm test'
            }
        }

        stage('Deploy Locally') {
            steps {
                // Deploy the app locally (for example, start the app)
                sh 'npm start &'
            }
        }
    }

    post {
        always {
            // Cleanup step, such as stopping the app if necessary
            sh 'pkill -f "npm start" || true'
        }
    }
}
