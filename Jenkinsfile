pipeline {
    agent any
    stages {
	stage('Work in specific directory') {
        steps {
			dir('e:\jenkins') { // Change directory to "my-git-folder"
                    dir // Execute a command within the specified directory
                }
            }
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/pmjadav/jenkin-demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
