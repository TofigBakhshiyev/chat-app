pipeline {
    agent any

    stages {
        stage('installations') {
            steps {
                echo 'Building..'
                nodejs('Node-15.2.0') {
                    sh 'yarn install'
                }
            }
        }
        stage('run app') {
            steps {
                echo 'App test..'
                withGradle() {
                    sh './gradlew -v'
                }
            }
        } 
    }
}
