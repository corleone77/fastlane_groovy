pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'fastlane deploy' 
            }
        }
    }
     stages {
        stage('Demo') {
           steps {
              sh 'fastlane instrumentation_tests'
                }
         }
        }	
}
