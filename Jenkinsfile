pipeline {
    agent any

    stages {
        stage('Build & Deploy') {
            steps {
                bat "mvn clean package"
            }
        }
	}
	post {
		success {
			withCredentials(usernamePassword(credentialsId: 'a53960cb-f047-4b6b-8bfd-09136a30352d'))
		}
	}
}
