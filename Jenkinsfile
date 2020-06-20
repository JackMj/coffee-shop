pipeline{
    agent any
    environment{
        PATH = "/opt/maven-3.6/bin:$PATH"
    }
    stages{
        stage("Maven Build") {
            steps{
                sh "mvn clean"
            }
        }
    }
}
