pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
				withMaven {
					sh "mvn clean verify"
					sh "mvn –version"
				}
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls
                '''
            }
        }
    }
}
