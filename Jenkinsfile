pipeline {
     agent any
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
           stage("deploy"){
               steps {
                    sh 'cp target/maven-web-application.war /opt/tomcat/webapps/'
               }
          }
     }
     } 
