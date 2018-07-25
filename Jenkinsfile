pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('DeployProd') {
#	when {
#                branch 'martinlegaspi'
#            }
	steps {
                echo 'Deploying production....'
            }
        }
#        stage('DeployDevelop') {
#	when {
#                branch 'develop'
#            }
#	steps {
#                echo 'Deploying develop....'
#            }
#	}
    }
}
