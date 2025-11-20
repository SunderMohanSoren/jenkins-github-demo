pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                checkout scm
            }
        }

        stage('Set Permissions') {
            steps {
                sh 'chmod +x hello.sh'
                sh 'chmod +x test.sh'
            }
        }

        stage('Run Script') {
            steps {
                sh './hello.sh'
            }
        }

        stage('Run Tests') {
            steps {
                sh './test.sh'
            }
        }
    }
}
