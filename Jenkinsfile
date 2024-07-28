pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000 --env NPM_CONFIG_REGISTRY=https://registry.npmmirror.com/' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
