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
                sudo mkdir -p /opt/myapp
                sudo cp -r * /opt/myapp/
                '''
            }
        }
    }
}
