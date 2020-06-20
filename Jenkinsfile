pipeline{
    agent any
    environment{
        PATH = "/opt/maven3/bin:$PATH"
    }
    stages{
        stage("Git checkout") {
            steps{
                git 'https://github.com/JackMj/coffee-shop.git'
            }
        }
        stage("Maven Build") {
            steps{
                sh "mvn clean package"
            }
        }
    }
}