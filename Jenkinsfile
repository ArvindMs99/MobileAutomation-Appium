pipeline {
    agent any
    stages {
        stage('BUILD') {
            steps {
                echo 'BUILDED'
            }
        }
        stage('DEPLOY') {
            steps {
                echo 'DEPLOYED'
            }
        }
        stage('TEST') {
            steps {
                bat 'cd android'
                bat 'cd testng-examples'
                bat 'mvn test -Dtest="FirstTest"'
                echo 'TESTED'
            }
        }
        stage('RELEASE') {
            steps {
                echo 'RELEASED'
            }
        }
    }
}
