
pipeline {
    agent any
	stages {
		stage ('config'){
			steps {
				sh "yum install httpd -y"
				sh "cp -r index.html /var/www/html"
				sh "chmod -r 777 /var"
			}
		}
		stage ('deploy'){
			steps{
				sh "systemctl restart httpd"
				}
			}
		}
	}
