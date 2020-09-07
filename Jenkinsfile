pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                input message: 'Upload file', parameters: [file(name: 'data.zip')]
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
