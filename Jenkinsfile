pipeline {
       agent any
       stages {
           stage('Clone Repository') {
               steps {
                   git 'https://github.com/nandhakrishna10/ngrok'
               }
           }
           stage('Install Dependencies') {
               steps {
                   sh 'pip install -r requirements.txt'
               }
           }
           stage('Run Tests') {
               steps {
                   sh 'pytest'
               }
           }
       }
   }
