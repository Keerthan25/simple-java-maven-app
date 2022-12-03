pipeline{
    agent any
    
    stages {
        stage('GIT checkout') {
			
            steps {
                echo 'This is slave1 agent'
                sh 'sleep 5'
			}
		}
        stage('Build stage') {
			
            steps {
                echo 'This is slave2 agent'
                sh 'sleep 5'
			}
		}
	}	
}
