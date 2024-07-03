pipeline {
    agent any
    stages {
        stage ('SCM checkout') {
            steps {
                script {
                    git 'https://github.com/vijayamalini2496/ecs-proj.git'
                }
            }
        }
        stage('Install dependencies') {
            steps {
                script {
                    // Install npm dependencies
                    sh 'npm install'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    // Run the npm build script
                    sh 'npm run build'
                }
            }
        }
    }
}
