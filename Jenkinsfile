pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') {
            steps {
                bat 'echo buildd project'
            }
        }
        stage('Test') {
            steps {
                echo 'Tests done'
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