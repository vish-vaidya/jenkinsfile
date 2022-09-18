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


	stage ('installing'){
	
		steps {
			sh "yum install httpd -y"
                        sh "service httpd start"
                        sh "chkconfig httpd on"
		}
	
	}

}

}
