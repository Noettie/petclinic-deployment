pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=445832677363.dkr.ecr.us-east-1.amazonaws.com/nottiey/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
