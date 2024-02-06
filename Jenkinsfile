pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn  -DskipTests  clean verify sonar:sonar -Dsonar.login=admin -Dsonar.password=habib'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
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
