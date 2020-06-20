pipeline{
    agent any
    environment{
        PATH = "/var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/M3/bin/mvn"
    }
    stages{
        stage("Git checkout") {
            steps{
                git branch: 'coffee-shop', url: 'https://github.com/JackMj/coffee-shop.git'
            }
        }
        stage("Maven Build") {
            steps{
                sh "mvn clean package"
            }
        }
    }
}