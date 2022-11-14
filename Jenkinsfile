pipeline{
    
    agent any

     tools {
        maven 'M3'
    }

    stages{

        stage('Git Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/jammey53/ci-cd.git'
            }
        }
        stage('build'){
        withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
    }
    }
}