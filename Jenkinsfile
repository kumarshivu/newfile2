pipeline {
    agent any
      environment {
          PATH="/opt/apache-maven-3.8.2/bin:PATH"
      }     
          stages {
        stage('SCM') {
            steps {
             git branch: 'main', url: 'git \'https://github.com/kumarshivu/newfile2.git\'' 
            }
        }
        stage('maven') {
            steps {
             sh "mvn package" 
            }
        }
    }   
}
