pipeline {
    agent any
    stages {
        stage ('SCM checkout') {
            steps {
                script{
                     git 'https://github.com/vijayamalini2496/ecs-proj.git'
                }
            }
        }
         stage ('Build') {
            steps {
                script{
                     sh 'npm install'
                }
            }
        }
}
}
