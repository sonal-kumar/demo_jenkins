pipeline {
    agent any
     tools {
        jdk 'JDK11'
    }
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}