pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                sh ('kubectl install && yarn install')
                echo 'Installing..'
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
