pipeline {
    agent any

    tools {
       nodejs "node"
    }

    stages {
		stage('Hello'){
			steps {
				echo "hello world"
				bat 'npm --version'
			}
		}
		
        stage('Git') {
            steps {
               git 'https://github.com/avneesh21/react-app.git';  
            }
        }
		
		stage('Build') {
			steps {
				bat 'npm install'
				bat 'npm start'
			}
		}
    }
}
