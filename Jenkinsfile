pipeline {
    agent any
    tools {
        nodejs 'NODE'
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
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


