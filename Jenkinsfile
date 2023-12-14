pipeline {
    agent any
    stages {
        stage('Install Apache') {
            steps {
                sh 'yum install httpd -y'
            }
        }
        stage('Start Apache') {
            steps {
                sh 'service httpd start'
            }
        }
        stage('Deploy Index') {
            steps {
                sh 'echo hello all >> /var/www/html/index.html'
            }
        }
    }
}
