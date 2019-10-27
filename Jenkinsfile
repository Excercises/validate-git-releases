pipeline {
    agent any

    stages {
        stage('Build & Deploy') {
            steps {
                bat "mvn clean package deploy"
            }
        }
	}
}
