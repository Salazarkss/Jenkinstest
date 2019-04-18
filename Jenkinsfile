pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps{
                withMaven(maven : 'maven_3_6_0'){
                    bat 'mvn clean package'
                }
            }
        }
        stage ('Deploy') {
            steps {
                withEnv(['GCLOUD_PATH=C:\Users\Sebastian\AppData\Local\Google\Cloud SDK\google-cloud-sdk\bin']) {
                    sh '$GCLOUD_PATH/gcloud --version'
                }
            }
        }
    }
}
