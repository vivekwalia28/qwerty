properties([parameters([string(defaultValue: '9', name: 'storeGroup'), string(defaultValue: '38100', name: 'dms'), choice(choices: ['preview'], name: 'environment')])])
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'sec', passwordVariable: 'password', usernameVariable: 'username')]) {
			sh '''
			echo "Hello"
			sh '''
}
            }
        }
        
    }
}
