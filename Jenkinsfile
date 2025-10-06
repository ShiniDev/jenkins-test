pipeline {
    agent any
    stages{
        stage('Greeting') {
            steps {
                echo 'Hello, World! Haba-desu pipeline!'
            }
        }
        
        stage('Show Current Location') {
            steps{
                echo 'Running pwd command:'
                sh 'pwd'
            }
        }
        
        stage('List files') {
            steps{
                echo 'Running ls command:'
                sh 'ls -la'
            }
        }
        
        stage('Simulate test') {
            steps{
                echo 'Simulating tests...'
                sh 'echo "All tests passed!"'
            }
        }
    }
    
    post{
        always {
            echo 'Pipeline finished.'
        }
    }
}