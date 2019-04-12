pipeline {
    agent { 
	docker {
		image 'corleone77/fastlane:v1'
		args ' -u root -v $RUTA:/app'}}

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
