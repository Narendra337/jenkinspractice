
pipeline {
    agent any

    stages {
       // stage('git-checkout') {
       //   steps {
       //     git branch: 'main', url: 'https://github.com/Narendra337/jenkinspractice.git'
      //     }
      //  }
        stage('stage1') {
            steps {
                sh 'terraform init'
            }
        }
        stage('stage2') {
            steps {
                sh 'terraform plan'
            }
        }
        stage('stage3') {
            steps {
                sh 'terraform apply -auto-approve '
            }
        }
    }
}
