
pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        },
        stage('Checkout'){
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5928295f-7cf6-41a5-b96e-1b9011fe3964', url: 'https://github.com/AWeckerlyONS/simple-app.git']]])
        }
    }
}