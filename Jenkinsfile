 pipeline {
    agent any

     stages {
        stage('Build') {
            steps {
	      bat "mvn -Dmaven.test.failure.ignore=true clean"
            }
	    }
        stage('test') {
            steps {
               bat "mvn clean test"
            }
        }
        stage('Package') {
            steps {
               bat "mvn package"
            }
        }
    }
}
 
