pipeline{
    agent any
    environment{
        PATH = "/opt/maven-3.6/bin:$PATH"
        DOCKER_TAG = getDockerTag()
    }
    stages{
        stage("Maven Build") {
            steps{
                sh "mvn clean"
            }
        }
        stage("Build Docker Image") {
            steps() {
                sh "docker build -t coffee-shop:${DOCKER_TAG} ."
            }
        }
    }
}

def getDockerTag() {
    def tag = sh script: 'git rev-parse HEAD', retirnStdout: true
    return tag
}
