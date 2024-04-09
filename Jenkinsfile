pipeline {
    agent any
    stages {
        stage("compile") {
            steps {
                // Use 'bat' step to execute commands on Windows
                bat 'javac Test.java'
            }
        }
        stage("run") {
            steps {
                // Use 'bat' step to execute commands on Windows
                bat 'java Test'
            }
        }
    }

    post{
        always{
            echo 'always'
        }
        success{
            echo 'success'
        }
        failure{
            echo 'failure'
        }
    }



}
