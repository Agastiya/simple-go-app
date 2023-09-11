node {
    docker.image('golang:alpine').inside('-u root -p 7000:7000') {
        stage('Build') {
            checkout scm
            sh 'go build'
        }
            stage('Test') { 
            sh 'go test' 
        }
    }
}