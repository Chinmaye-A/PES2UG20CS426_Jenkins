pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS426-1 try.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS426-1'
            }
        }
    }
    post {
        always {
            ech 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
