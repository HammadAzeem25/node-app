pipeline {
    agent any
    stages {
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
        }
				stage('IntegrationTests') {
				 steps {
				        sh 'npm run unittest'
								}}
				stage('Integrationtest')
				{
             steps {
             sh 'npm run integrationtest'
				}
				}}
				}
