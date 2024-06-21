pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
        // Add more stages as needed (e.g., test, deploy, etc.)
    }
}
