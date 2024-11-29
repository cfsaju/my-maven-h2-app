pipeline {
    agent any

    tools {
        maven 'mvn39'
        
    }

    stages {
        stage('Compile') {
            steps {
               sh "mvn compile"
            }
        }

        stage('Test') {
            steps {
                sh "mvn test"
            }
        }

        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
