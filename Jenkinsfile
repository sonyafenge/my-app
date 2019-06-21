pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
             //   sh "rm -rf my-app"
             //   sh "git clone https://github.com/sonyali03/my-app.git"
                sh "mvn clean "
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test " 
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package "
            }
        }
    }
}
