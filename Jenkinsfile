pipeline {
    agent any
    stages {
        stage('SCM') {

            steps {

                       git "https://github.com/saurabhsonje/alldone.git"
                //

            }

        }

        stage('Test') {

            steps {

                sh "mvn test"

                //

            }

        }

        stage('Deploy1') {

            steps {

                  sh "/nexus/sonar-scanner-3.3.0.1492-linux/bin/sonar-scanner"


            }

        }

                  stage('Deploy2') {

            steps {

                  sh "mvn clean deploy"
            }

        }
                      stage('Deploy3') {

            steps {
                       echo "this is step1"

             
            }

        }

    }

}






