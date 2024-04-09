pipeline {
    agent any
    environment{
        VERSION_NAME="1.34"
    }


    stages {
        stage("compile") {
            steps {
                // Use 'bat' step to execute commands on Windows
                bat 'javac Test.java'
                echo '${VERSION_NAME}'
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
