pipeline {
    agent any

    environment {
        GITHUB_CRED = credentials('github-cred')
        DOCKER_CRED = credentials('docker-server-cred')
        DOCKER_HOST = "13.250.37.220"
        DOCKER_USER = "ubuntu"   // replace with your Docker server username
        APP_NAME = "my-app"
        JAR_FILE = "target/my-app-1.0-SNAPSHOT.jar"
        IMAGE_NAME = "my-app-image"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Deena7/my-project.git',
                    credentialsId: 'github-cred'
            }
        }
      }
    }
