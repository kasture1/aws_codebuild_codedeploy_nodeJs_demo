pipeline {
    agent any
    tools {nodejs "mynodejs"}
    stages {
        stage('Dev') {
            steps {
                git 'https://github.com/kasture1/aws_codebuild_codedeploy_nodeJs_demo.git'
                echo 'Below is index.js file'
                sh 'cat index.js'
            }
        }
     stage('Build') {
            steps {
                sh 'npm install'
                echo 'Success'
            }
        }
    }
}