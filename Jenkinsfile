@Library('sharedlib') _
def tools = new org.devops.tools()
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script {
                tools.PrintMes('this is a test from mylib')      
                }
              
            }
        }
    }
}
