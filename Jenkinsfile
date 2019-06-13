pipeline {
    agent any
    
    stages {
        stage('Preparation') {
            steps{
                echo "Preparation"   
            }
        }
        stage('Build') {
            steps{
                echo "Build"
                ls
                sh ./gradlew clean test jar
            }
        }
        stage('Results') {
            steps{
                echo "Results"
                ls
            }
        }
    }
}
