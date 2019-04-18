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
            steps{
                withEnv(["GCLOUD=\\Users\\Sebastian\\AppData\\Local\\Google\\Cloud SDK\\google-cloud-sdk\\bin"]){
                    sh 'gcloud --version'
                }
            }
        }
    }
}
