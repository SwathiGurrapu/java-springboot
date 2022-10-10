pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Build'
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
                sh 'mvn test'
            }
        }
         stage('Sonarqube') {
            steps {
                echo 'Sonarqube'
            }
        }
         stage('Push to artifactory') {
            steps {
                echo 'Push to artifactory'
            }
        }
         stage('Deploy to QA') {
            steps {
                echo 'Deploy to QA'
            }
        }
         stage('Deploy to Prod') {
            steps {
                echo 'Deploy to Prod'
            }
        }  
    }

    post { 
        success { 
            echo 'success!'
        }
         failure { 
            echo 'Failed!'
        }
         always { 
            echo 'always'
        }
    }
}