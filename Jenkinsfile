 pipeline {
        agent any

        stages {
                stage('create image') {
                        steps {
                                sh 'docker build -t pipeimage .'
                        }
                
                     }
               stage('create container') {
                        steps {
                                sh 'docker run -dit --name Jen-docker-p1 -p 4000:80 pipeimage'
                        }
                
                     }
                }
       }
