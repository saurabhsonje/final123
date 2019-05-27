pipeline {
    agent any
    stages {
        stage('SCM') {

            steps {

                       git "https://github.com/saurabhsonje/nexusdata.git"
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

                  sh "/nexus"


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






