pipeline {
    agent any
    tools {
        maven 'mvn'  // This must match the Maven name in Jenkins Global Tool Configuration
    }

    stages {
        stage('Pull code') {
            steps {
                git branch: 'main', url: 'https://github.com/iam-aniketmore/DevopsProject2.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
