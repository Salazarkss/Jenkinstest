node {
    stage('SCM Checkout'){
        git 'https://github.com/Salazarkss/Jenkinstest'
    }
    stage('Compile'){
        sh 'mvn clean package'
    }
}