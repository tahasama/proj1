pipeline {
    agent { //none
        docker { image 'python:3.9' }
    }

    stages {
        stage('Build') {
            //agent {
              //  docker { image 'python:3.9' }
                //}
            
            steps {
                
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Test') {
            //agent any
            steps {
               // sh 'docker-compose -v'
               // sh 'docker-compose run web python manage.py test ./app'
                sh ' python app/manage.py test ./app'
            }
        }
        stage('Deploy') {
            //agent any
            steps {
                
                 sh 'echo not yet...taha...wa touhou'
            }
        }
    }
}
