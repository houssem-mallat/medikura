pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                echo 'Installing 5 ...'
                //Installing kubectl in Jenkins agent
                sh 'curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl'
                sh 'sudo chmod +x ./kubectl && sudo mv kubectl /usr/local/sbin'
                //Clone git repository
                git url:'https://github.com/houssem-mallat/medikura.git'
                
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
