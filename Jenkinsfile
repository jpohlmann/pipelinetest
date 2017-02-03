pipeline {
    agent any // <1>

    stages {
        stage('Build') { // <2>
            steps { // <3>
                echo 'make' // <4>
            }
        }
        stage('Test'){
            steps {
                echo 'testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploying'
            }
        }
    }
}
