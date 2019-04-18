pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps{
                withMaven(maven : 'maven_3_6_0'){
                    bat 'mvn clean package && cd && mvn appengine:deploy'
                }
            }
        }
    }
}
