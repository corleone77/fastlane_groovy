pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo test' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
