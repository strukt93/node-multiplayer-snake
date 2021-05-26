node('master'){
	def app
	stage('Cloning Git'){
		checkout scm
}
	stage('Build-and-Tag'){
		app = docker.build('strukt93/snake:test')
}
	stage('Post-to-dockerhub'){
		docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
			app.push('test')
	}
}
	stage('Pull-image-server'){
		sh "whoami && echo $PATH"
		sh "/usr/local/bin/docker-compose down"
		sh "/usr/local/bin/docker-compose up -d"
}
}
