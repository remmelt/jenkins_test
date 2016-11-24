#!groovy

pipeline {
    agent any

    stages {
        stage("Checkout") {
            steps {
                sh 'echo ok ok ok'
            }
        }

        stage("Hoei") {
            steps {
                parallel (
                    "One": {
                        sh 'echo dubbele hoei'
                        sh 'sleep 3'
                        sh 'echo End ONE'
                    },
                    "Two": {
                        sh 'echo dubbele hoei2'
                        sh 'sleep 3'
                        sh 'echo End TWO'
                    }
                )
            }
        }

        stage("Deploy") {
            steps {
                sh 'deployen maar!'
                sleep 5
                echo 'so done with this'
            }
        }
    }
}
