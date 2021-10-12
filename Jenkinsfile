properties([parameters([string(defaultValue: '9', name: 'STOREGROUP'), string(defaultValue: '38100', name: 'DMS'), choice(choices: ['PREVIEW'], name: 'ENVIRONMENT')])])
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
