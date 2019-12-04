pipeline {
    agent any
        stages {
            stage('Build') {
                steps {
                    sh('echo Building')
                }
            }
            stage('Test') {
                steps {
                      sh('echo Testing')
                }
            }
            stage('Deploy') {
                when {
                    branch 'master'
                }
                steps {
                    sh('echo Deploying')
                }
            }
    }
}
