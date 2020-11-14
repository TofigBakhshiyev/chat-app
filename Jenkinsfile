pipeline {
    agent any
    
    tools {
        gradle 'Gradle-6.2'
    }
    
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
                sh './gradlew -v'
            }
        } 
    }
}
