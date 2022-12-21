
pipeline {
	agent {
		label {
			label 'built-in'
			customeWorkspace "/mnt/pipe-job"
			}
		}
	stages {
		stage ('config'){
			steps {
				sh "yum install httpd -y"
				sh "cp -r index.html /var/www/html/index"
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
