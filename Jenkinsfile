pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy') {
            steps {
                
                sh 'cp -f target/typing-game.war /opt/tomcat9/webapps/'
            }
        }
    }
}
