pipeline {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello World'
         }
      }
	  stage('Git Repository') {
         steps {
            git "https://github.com/sreedhar-guntala/sreemavenproject.git"
         }
      }
	  stage('clean') {
         steps {
            sh "mvn clean"
         }
      }
	  stage('test') {
         steps {
            sh "mvn test"
         }
      }
	  stage('package') {
         steps {
            sh "mvn package"
         }
      }
   }
}