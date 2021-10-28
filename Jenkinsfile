pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
				mvn clean install;
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
				ls;
            }
        }
    }
}
