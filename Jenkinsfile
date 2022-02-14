pipeline {
    agent any

    stages {
        stage('hello') {
            steps {
                sh "echo hello"
            }
        }
	stage('cat Readme') {
	    when {
	      branch "fix-*"
	    }
	    steps {
	        sh '''
		  cat Readme.md
		'''	
	    }
	}
    }
}
