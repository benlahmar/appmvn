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
                bat 'mvn Test'
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
