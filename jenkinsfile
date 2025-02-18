pipeline {
    agent any

    environment {
        GITHUB_CREDENTIALS = credentials('github creds')  // Use stored GitHub credentials
    }

    stages {
        stage('Checkout Code') {
            steps {
                echo "Cloning repository..."
                git branch: 'main', 
                    url: 'https://github.com/gillsanjeev/Website-PRT-ORG.git',
                    credentialsId: 'github creds'
            }
        }
    }
}
