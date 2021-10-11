pipeline {
    agent any

    stages {
        stage('Build') {
          environment {
            SECRET_FILE_ID = credentials('secret-file')
       }
            steps {
                echo 'Building..'
                echo "####DISPLAYING SECRET_FILE_ID####"
	              echo "Global property file: ${SECRET_FILE_ID}"
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
