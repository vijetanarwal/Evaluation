pipeline {
    agent any
    tools {
        nodejs 'NODE'
    }
    stages {
        stage('Build') {
            steps {
                echo 'build successful'
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