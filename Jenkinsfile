pipeline {
agent any
stages {
    stage('Build') {
        steps {
            echo'build successful'
        }
    }
    
    stage('Test') {
        steps {
            echo 'test successful'
        }
    }
    
    stage('Deploy') {
        steps {
            // deployment code
            echo 'deployment successful'
        }
    }
}

post {
    always {
        script {
            if (currentBuild.result == "FAILURE") {
                echo "Pipeline failed"
            }
        }
    }
}
}
