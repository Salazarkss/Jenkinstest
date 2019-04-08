
pipeline {
	agent {
		label 'docker' 
	}

    agent {
    	docker{
    		label: 'docker',
    		image 'maven:3.3.3'
    	}
    }

    stages {
        stage('build') {
            steps {
                sh 'mvn package && gcloud app deploy'
            }
        }
    }
}