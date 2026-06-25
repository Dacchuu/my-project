pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Deploy to Folder') {
            steps {
                sh '''
                mkdir -p /opt/myapp
                cp -r * /opt/myapp/
                '''
            }
        }
    }
}
