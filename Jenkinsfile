pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Run Hello Script') {
            steps {
                sh 'bash scripts/hello.sh'
            }
        }

        stage('Run Build Script') {
            steps {
                sh 'bash scripts/build.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}
