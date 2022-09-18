pipeline {
agent {

node {
			label 'node1'
			customWorkspace '/mnt/file'

}

}

stages {

	stage ('GIT'){
	
		steps {
				sh "sudo yum install git -y"
        sh "git init"
        sh "git remote add origin https://github.com/vish-vaidya/jenkinsfile.git"
		}
	
	}

}

}
