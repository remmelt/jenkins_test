#!groovy

pipeline {
    agent any

    stages {
        stage("Checkout") {
            checkout scm
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
    }
}
