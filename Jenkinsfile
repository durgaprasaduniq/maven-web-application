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
           stage("deploy"){
               steps {
                    sh 'cp /home/ec2-user/GREATCODER/GREATCODER/workspace/multi-config_master/target/maven-web-application.war /home/ec2-user/apache-tomcat-9.0.115/webapps/ROOT.war'
               }
          }
     }
     } 
