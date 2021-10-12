properties([parameters([string(defaultValue: '9', name: 'storeGroup'), string(defaultValue: '38100', name: 'dms'), choice(choices: ['preview'], name: 'environment')])])
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                withCredentials([usernamePassword(credentialsId: 'sec', passwordVariable: 'password', usernameVariable: 'username')]) {
			sh '''
			echo $user >> test.txt
			echo $pass >> test.txt
			cat test.txt
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
