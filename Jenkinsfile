pipeline {
    agent any
    triggers { pollSCM 'H/5 * * * *'}
    tools {
    maven "apache-maven"
    jdk "JDK"
    }
    
    stages {
    stage('Maven Build') {
        steps {
        bat "mvn clean compile"
            }
        }
    }
}
