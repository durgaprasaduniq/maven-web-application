pipeline {
     agent {label "JENKINS"
} 
       stages {
         stage("get the code") {
            steps {
               git 'https://github.com/durgaprasaduniq/maven-web-application.git'
            }
         }
          stage("build the code"){
              steps {
                sh 'mvn clean package'
          }
      } 
    }
}
