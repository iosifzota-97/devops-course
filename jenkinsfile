pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				withMaven(maven : 'MAVEN_HOME') {
					sh 'mvn clean compile'
					sh 'mvn package shade:shade'
				}
			}
		}
	}
}
