@Library('sharedlib') _
def tools = new org.devops.tools()
pipeline {
        agent {
        docker {image 'hongxuhematt/myubuntu:2.0'}
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script {
                tools.PrintMes('this is a test from mylib')      
                pwsh 'Write-Host "Hello from PowerShell inside Docker!"'
                }
              
            }
        }
    }
}
