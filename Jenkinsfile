pipeline{
    agent any
    stages{

        stage('Clone Code')
        steps{
                git 'https://github.com/winnerJd/devops-demo.git'
        }
    }
    stage('Build Docker Image'){
        steps{
                sh 'docker build -t devops-demo:latest .'
        }
    }
    stage('Run Container'){
        steps{
sh 'docker run --rm -d devops-demo'        }
    }
}