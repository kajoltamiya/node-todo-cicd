pipeline {
    agent any
    
    stages {
        
        stage("code"){
            steps{
                git url: "https://github.com/kajoltamiya/node-todo-cicd.git", branch: "master"
                echo 'code has been cloned'
            }
        }
        stage("build and test"){
            steps{
                sh "docker build -t node-app-test-new ."
                echo 'code has been build'
            }
        }
        stage("scan image"){
            steps{
                echo 'image Scanned'
            }
        }
        
    }
}
