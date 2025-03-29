pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'No tests defined'
            }
        }
        stage('Deploy') {
            steps {
                echo 'App will be deployed'
            }
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