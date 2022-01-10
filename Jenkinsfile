pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
stage('Checkout SCM') {
            steps {
                checkout([
                 $class: 'GitSCM',
                 branches: [[name: 'hotfix']],
                 userRemoteConfigs: [[
                    url: 'https://github.com/HammadAzeem25/node-app',
                    credentialsId: '',
                 ]]
                ])
            }
        }}
				}
