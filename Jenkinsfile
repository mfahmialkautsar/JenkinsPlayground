pipeline {
    agent any
    tools {
        maven 'maven'
        jdk 'jdk21'
    }
    stages {
        stage('env') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install -B --no-transfer-progress'
            }
        }
    }
}
