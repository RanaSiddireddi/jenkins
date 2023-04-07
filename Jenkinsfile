pipeline {
    agent any

    environment {
        SSH_CRED = credentials('SSH_CRED')
    }

    stages {
        stage('one') {
            steps {
                echo "i am step one stage one"
                echo " details are ${SSH_CERD}"
            }
        }
        stage('two') {
            steps {
                echo "i am step one stage two"
            }
        }
        stage('three') {
            steps {
                echo "i am step one stage three"
            }
        }
    }
}

