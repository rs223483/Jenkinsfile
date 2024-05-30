    pipeline{
    agent any
    stages{
        stage("echo a line"){
            steps{
                echo "This is first line"
            }
        }
        stage("Run pwd command"){
            steps{
                sh 'pwd'
            }
        }
        stage("Runnig multiple commands"){
            steps{
                sh '''pwd
                    ls
                    whoami'''
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
