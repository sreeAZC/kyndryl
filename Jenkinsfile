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
                                sh 'docker run -dit --name Jen-docker-p2 -p 4002:80 pipeimage'
                        }
                
                     }
                }
       }
