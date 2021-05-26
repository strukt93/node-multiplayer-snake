node('master'){
	def app
	stage('Cloning Git'){
		sh "curl -L https://github.com/docker/compose/releases/download/1.17.0/docker-compose-`uname -s`-`uname -m` -o /tmp/docker-compose"
		sh "chmod +x /tmp/docker-compose"
		sh "/tmp/docker-compose"
		//checkout scm
}/*
	stage('Build-and-Tag'){
		app = docker.build('strukt93/snake:test')
}
	stage('Post-to-dockerhub'){
		docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
			app.push('test')
	}
}
	stage('Pull-image-server'){
		sh "which docker-compose && ls /usr/local/bin"
		sh "docker-compose down"
		sh "docker-compose up -d"
}*/
}
