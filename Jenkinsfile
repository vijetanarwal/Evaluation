pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            bat 'mvn clean package'
        }
        stage('Test') {
            bat 'mvn test'
            echo 'No tests'
        }
        stage('Deploy') {
            bat 'echo app will be deployed'
        }
    }
    post {
        always{
            echo 'ALWAYS'
        }
        success{
            echo 'only when above stages runs'
        }
        failure{
            echo 'FAIL'
        }
    }
}