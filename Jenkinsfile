pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
				withMaven {
					sh "clean install"
				}
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls
                '''
				sh "echo "POM_VERSION=$(grep -v '\[' version.log)" > props.properties"
            }
        }
    }
}
