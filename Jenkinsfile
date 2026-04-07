pipeline{
    agent any
    stages{

        stage('Clone Code')
        steps{
                git 'https://github.com/your-repo/devops-demo.git'
        }
    }
    stage('Build Docker Image'){
        steps{
                sh 'docker build -t devops-demo:latest .'
        }
    }
    stage('Run Container'){
        steps{
                sh 'docker run  devops-demo'
        }
    }
}