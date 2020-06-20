pipeline{
    agent any
    environment{
        PATH = "/var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/M3/bin/mvn"
    }
    stages{
        stage("Maven Build") {
            steps{
                sh "mvn clean install"
            }
        }
    }
}