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
		sh "docker-compose down"
		sh "docker-compose up -d"
}
}
