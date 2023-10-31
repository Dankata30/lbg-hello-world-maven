pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M3"
    }

    stages {
        stage('Checkout') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'main', url: 'https://github.com/Dankata30/lbg-hello-world-maven.git'
            }
        }
        
        stage('Compile') {
            steps {
                // Get some code from a GitHub repository
                sh 'mvn clean compile'
            }
        }
        
        stage('Final Stage') {
            steps {
                // Get some code from a GitHub repository
                sh 'echo "final stage"'
            }
        }
    }
}
