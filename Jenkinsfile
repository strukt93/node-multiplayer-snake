node('master'){
	def app
	stage('Cloning Git'){
		checkout scm
}
	stage('Build-and-Tag'){
		sh "echo Build-And-Tag"
		//app = docker.build('strukt93/snake:test')
}
	stage('Post-to-dockerhub'){
		sh "echo Post-to-Dockerhub"
		/*docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
			app.push('test')*/
}
}
	stage('Pull-image-server'){
		sh "Pull-image-server
		/*sh "docker-compose down"
		sh "docker-compose up -d"*/
}
}
