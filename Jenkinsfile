pipeline {
agent {

node {
			label 'node1'
			customWorkspace '/mnt/file'

}

}

stages {

	stage ('copy index'){
	
		steps {
				sh "cp -r index.html /var/www/html/"
		}
	
	}


	stage ('copy dev'){
	
		steps {
				sh "cp -r dev.html /var/www/html/"
		}
	
	}

	stage ('copy QA'){
	
		steps {
				sh "cp -r qa.html /var/www/html/"
		}
	
	}

}

}
