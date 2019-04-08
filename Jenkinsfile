pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'fastlane deploy' 
            }
        }
    
       stage('Demo') {
           steps {
              sh 'fastlane instrumentation_tests'
              }
         }
     }	
}
