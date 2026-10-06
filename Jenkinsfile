pipeline {
    agent any
    stages{
        stage('clean'){
            steps {
                sh "chmod -R 777 /var/www/html"
                sh "rm -rf /var/www/html/index.html"
                sleep 5
            }
        }
        stage('pasting in /var/www/html'){
            steps {
                sh "cp -r index.html /var/www/html"
                sleep 5
            }
        }
        stage('launch'){
            steps {
               sh "chmod -R 777 /var/www/html"
              echo "launch url now"
            }
        }
    }
}
