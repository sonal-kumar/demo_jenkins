pipeline {
    agent any
     tools {
        jdk 'JDK11'
    }

	stages 
	{
        stage('build') {
            steps {
                echo 'Building the source'
                sh 'mvn clean compile'
            }
        }
        stage('test') {
            steps {
                echo 'Testing source'
                sh 'mvn test'
            }
        }
		stage('deploy') {
            steps {
                echo 'packaging'
                sh 'mvn package'
            }
        }


	}

}