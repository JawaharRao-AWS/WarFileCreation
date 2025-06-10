pipeline{
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages{
        stage("Git Cloning"){
            steps{
                git url: "https://github.com/JawaharRao-AWS/war-web-project.git", branch: "master"
            }
        }
        stage("Building"){
            steps{
              sh "mvn clean package"
            }
        }
    }
}
 
