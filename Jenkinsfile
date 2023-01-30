pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
         stage('docker_verify') {
            steps {
                echo 'docker --version'
            }
        }
        stage('docker_image') {
            steps {
                echo 'sudo docker build -t myimage:v1 .'
            }
        }
        stage('Docker_image_verifycation') {
            steps {
                sh 'sudo docker images'
                sh 'echo "i am due to webhook"'
            }
        }
    }
}
