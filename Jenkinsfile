pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Build Completed."'
            }
        }
    }
    post {
        always {
            script {
                currentBuild.description = "Started at: ${env.BUILD_TIMESTAMP}"
            }
        }
    }
}
