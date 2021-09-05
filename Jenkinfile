pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build the project'
            }
        }
		stage('Test') {
            steps {
                echo 'Test the project'
            }
        }
		stage('Deploy') {
            steps {
                echo 'Deploy the project'
            }
			
        }
    }
	 post {
        always {
            emailext body: 'status', subject: 'Pipeline status', to: 'rajusfort@gmail.com'
        }
    }
}
