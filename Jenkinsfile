pipeline {
    agent any
    triggers { pollSCM 'H * * * *'}
    tools {
    maven "apache-maven"
    jdk "JDK"
    }
    
    stages {
    stage('Checkout') {
        steps {
        git branch: 'main', url: 'https://github.com/jonesong1/Comp367_lab2_CICDv2.git'
            }
        }
    stage('Maven Build') {
        steps {
        bat "mvn clean compile"
            }
        }
    }
}
