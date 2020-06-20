pipeline{
    agent any
    environment{
        PATH = "/opt/maven-3.6/bin/"
    }
    stages{
        stage("Maven Build") {
            steps{
                sh "mvn clean"
            }
        }
    }
}
