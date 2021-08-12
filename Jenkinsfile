pipeline {
    agent any

    stages {
        stage('Build only fix branch') {
	  when {
	    branch "fix-*"
	  }
            steps {
                echo 'Building.. repo 1 only for branch fix'
            }
        }
        stage('Build only Pull Request') {
	  when {
            branch 'PR-*' 
	  } 
            steps {
                echo 'Building.. repo 1 only for PR'
            }
        }
	stage('Testing') {
	    steps {
                echo 'Testing.... repo 1'
	    }
	}    
        stage('Deploy') {
            steps {
                echo 'Deploying.... repo 1'
            }
        }
    }
}
