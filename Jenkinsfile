#!groovy​
pipeline {
    agent {
        kubernetes {
            label 'vscodenodeprofiler-buildpod'
            yaml """
apiVersion: v1
kind: Pod
spec:
  containers:
  - name: vscodenodeprofiler-builder
    image: node:lts
    tty: true
    command:
      - cat
"""
        }
    }

	 options {
        timestamps()
        skipStagesAfterUnstable()
    }

    stages {
        stage('Build') {
			steps {
				echo 'Building..'
				container("vscodenodeprofiler-builder") {
					sh '''
					#npm install
					#npm i vsce
					#npx vsce package
					echo "Extension build complete"
					ls -la
				'''
				}
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