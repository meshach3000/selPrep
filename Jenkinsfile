pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'mvn -B -DskipTests clean package'
                    } else {
                        bat 'mvn -B -DskipTests clean package'
                    }
                }
            }
        }
        // Add more stages as needed (e.g., test, deploy, etc.)
    }
}
