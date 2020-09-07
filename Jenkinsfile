pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "First Step"'
            }
        }
        
        stage('Test') {
            steps {
                input 'Proceed Second Step?'
                sh 'echo "Second Step"'
            }
        }
        
        
        stage('Deploy') {
            steps {
                sh 'echo "Third Step"'
            }
        }
    }
}
