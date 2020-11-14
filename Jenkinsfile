pipeline {
    agent any

    stages {
        stage('installations') {
            steps {
                echo 'Building..'
                nodejs('Node-14.0.0') {
                    sh 'yarn install'
                }
            }
        }
        stage('run app') {
            steps {
                echo 'App test..'
                withGradle() {
                    sh 'yarn start'
                }
            }
        } 
    }
}
