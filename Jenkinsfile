pipeline{
    
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/jammey53/ci-cd.git'
            }
        }
        stage('Unit Testing'){
            steps{
                sh 'mvn test'
            }
        }
    }
}