node {
	stage ('Checkout Repository') {
		deleteDir()
		checkout scm
	}

	stage ('Render Configurations') {
		sh 'ansible-playbook generate_configurations.yaml'
	}

	stage ('Unit Testing') {
		// Do something...
	}

	stage ('Deploy Configurations to Dev') {
		// Push the configurations out to the dev environment
	}

	stage ('Functional/Integration Testing') {
		// Ping some stuff
	}

	stage ('Promote Configurations to Production') {
		// Promote some things
	}

	stage ('Production Functional/Integration Testing') {
		// Ping some stuff
	}
}
