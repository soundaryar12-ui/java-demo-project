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
                sh 'sudo -n /usr/bin/cp target/tomcat-demo.war /opt/tomcat/webapps/tomcat-demo.war'
            }
        }
    }
}
