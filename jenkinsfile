@Library('simple-lib') _

pipeline {
    agent any

    stages {
        stage('Test Shared Library') {
            steps {
                script {
                    sayHello("Amigo")

                    def result1 = calculator.add(5, 3)
                    def result2 = calculator.multiply(4, 2)

                    echo "5 + 3 = ${result1}"
                    echo "4 * 2 = ${result2}"
                }
            }
        }
    }
}
