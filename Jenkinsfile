pipeline {
    agent any
    stages {
        stage('clone step') {
            steps {
                sh 'rm -rf hello-world-war'
                sh 'git clone https://github.com/venkibiligere/hello-world-war.git'
            }
        }
		stage('Build') {
            steps {
                sh 'mvn package'
            }
		}
		stage('Deploy step') {
            steps {
                 sh 'sudo cp /var/lib/jenkins/workspace/Multibranch_Config_Dev/target/hello-world-war-1.0.0.war
             }
        }
    }
}
