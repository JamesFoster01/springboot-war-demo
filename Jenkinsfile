pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '/opt/homebrew/bin/mvn clean'
                sh '/opt/homebrew/bin/mvn compile'
            }
        }

        stage('Package') {
            steps {
                sh '/opt/homebrew/bin/mvn package'
            }
        }
    }
}