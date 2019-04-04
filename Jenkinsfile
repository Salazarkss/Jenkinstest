
pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn package && java -jar target/gs-spring-boot-0.1.0.jar'
            }
        }
    }
}