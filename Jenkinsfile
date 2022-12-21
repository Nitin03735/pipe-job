
pipeline {
    agent any
	stages {
		stage ('config'){
			steps {
				sh "yum install httpd -y"
				}
		}
		stage ('deploy'){
			steps{
				sh "systemctl restart httpd"
				}
			}
		}
	}
