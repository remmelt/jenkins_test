pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: true, description: '', name: 'flag')
    }

    stages {
        stage("foo") {
            steps {
                echo "flag: ${env.FLAG}"
            }
        }
    }
}
