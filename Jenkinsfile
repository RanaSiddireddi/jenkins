pipeline {
    agent {
        label 'ANSIBLE'
    }

    environment {
        SSH_CRED = credentials('SSH_CRED')
    }

    stages {
        stage ('parallel-stage'){
            parallel {
                stage('one') {
                    steps {
                        echo "i am step one stage one"
                        echo "details are not shown here"
                    }
                }
                stage('two') {
                    steps {
                        echo "i am step one stage two"
                        sh "hostname"
                    }
                }
                stage('three') {
                    steps {
                        echo "i am step one stage three"
                    }
                }
            }
        } 
    }
}

