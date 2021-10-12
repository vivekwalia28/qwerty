pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                withCredentials([usernamePassword(credentialsId: 'sec', passwordVariable: 'pass', usernameVariable: 'user')]) {
			sh '''
			echo $user
			echo $pass
			sh '''
}
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
}
