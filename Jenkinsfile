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
                sh 'echo "hello everyone changes are deploy in file" >> /var/www/html/index.html'
            }
        }
    }
}
