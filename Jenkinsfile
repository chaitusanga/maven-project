pipeline {
	agent  any

	stages {
		stage('Build') {
			steps {
				sh '/Users/csanga/Documents/apache-maven-3.6.3/bin/mvn clean package'
				sh '/usr/local/bin/docker buid . -t tomcatwebapp:${env.BUILD_ID}'
			}
		}

	}
}