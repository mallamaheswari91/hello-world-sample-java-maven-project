pipeline {
    agent any
    
   
    stages {
        
        
          stage('Deployment') {
            steps {
                sshagent(['deployment-tamcat']) {
             sh  "scp  -o StrictHostKeyChecking=no /var/lib/jenkins/workspace/build_job/webapp/target/webapp.war ec2-user@54.252.152.98:/opt/apache-tomcat-9.0.73/webapps "      
}
             
            }
        }    
    }
}
