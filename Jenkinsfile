#!groovy​
pipeline {
    agent any

	 options {
        timestamps()
        skipStagesAfterUnstable()
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
				sh '''
					#npm install
					#npm i vsce
					#npx vsce package
					echo "Extension build complete"
					ls -la
				'''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}