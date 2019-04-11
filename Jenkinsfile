pipeline {
    agent { 
	docker {
		image 'docker.nespresso.com/fastlane:1.0'
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
