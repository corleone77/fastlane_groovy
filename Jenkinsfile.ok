pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'fastlane deploy' 
            }
        }
    
       stage('test') {
           steps {
              sh 'fastlane test'
              }
         }
     }	
}
