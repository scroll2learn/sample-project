@Library('jenkins-shared-library') _

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                buildApp()
            }
        }

        stage('Test') {
            steps {
                testApp()
            }
        }

        stage('Deploy') {
            steps {
                deployApp('development')
            }
        }
    }
}
