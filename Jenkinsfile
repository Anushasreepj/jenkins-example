pipeline {
    agent any

    stages {
        stage('Build Another Application') {
            steps {
                
                sh 'mvn clean install' 
            }
        }

        stage('Open Application') {
            steps {
                  
                def tomcatwebappsDir = "/home/ec2-user/apache-tomcat-8.5.93/webapps"
                def warFilePath ="${tomcatwebappsDir}${warFileName}"
                def warFileName = 'gameoflife.war' 
                def appUrl = "http://54.153.158.154:8088//${gameoflife.war}" 
                bat "start ${http://54.153.158.154:8088 }"
            }
        }
    }

    post {
        success {
            echo 'Build and opening successful'
        }
        failure {
            echo 'Build and opening failed'
           
        }
    }
}




    
