pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build World'
            }
        }
        stage('Test') {
            steps {
                echo 'Test World'
            }
        }
        stage('Deploy') {
            steps {
                echo0 'Deploy World'
            }
        }
    }
    
    post
    {
        always
        {
            emailext body: 'status', subject: 'pipeLine run', to: 'sakshishrivastav134@gmail.com'
        }
        failure
        {
            echo 'failed'
        }
    }
}
