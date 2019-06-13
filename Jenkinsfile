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
                sh "ls -a"
                sh "./gradlew clean test jar"
            }
        }
        stage('Results') {
            steps{
                echo "Results"
                sh "ls -a"
            }
        }
    }
}
