pipeline {
    agent any
    parameters{
        booleanParam(name: 'executeBuild', defaultValue: false, description: '')
    }

    stages {
        stage('build') {
            when {
                expression {
                    params.executeBuild
                }
            }
            steps {
                echo 'building the application..'
                
            }
        }
         stage('Test') {
                steps {
                    echo "Testing the application"
            }
        }
        stage("deploy") {
            steps {
                echo "deploying the application"
                
            }
        }
    }
}

