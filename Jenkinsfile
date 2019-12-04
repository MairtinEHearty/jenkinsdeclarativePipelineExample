pipeline {
    agent any
        stages {
            stage('Build') {
                steps {
                    echo 'Building'
                }
            }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('PR-Generated Against Master'){
          when {
              changeRequest target: 'master'
              }
          steps {
              echo 'PR raised against master branch'
          }
        }
        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}
