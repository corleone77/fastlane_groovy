pipeline {
    agent { docker {image 'reginfell/fastlane'}}

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
