pipeline {
  /* Declarative Pipeline
  @autor: Jaime Gaona */
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building ${env.BUILD_NUMBER} "
            }
        }
        stage('Analyze') {
            steps {
                echo 'Analyze..'
                /* make analyze */
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                /* make test */
            }
        }
        stage('Deploy to Stage') {
            /* when {
              branch master
            }*/
            steps {
                echo 'Deploying to staging'
                /* make staging */
            }
        }
        stage('Deploy to Production') {
           /* when {
              expression {
                currentBuild.result == null || currentBuild.result == 'SUCCESS'
              }
            }*/
            steps {
                echo 'Deploying to prod'
            }
        }
    }
}
