pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean -DskipTests package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
