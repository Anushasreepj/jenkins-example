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
                script {  
                def tomcatwebappsDir ="/home/ec2-user/apache-tomcat-8.5.93/webapps"
                def warFileName = 'gameoflife.war' 
                def warFilePath ="${tomcatwebappsDir}${warFileName}"
                def appUrl = "http://54.153.158.154:8088/gameoflife.war/" 
                open appUrl
            }
            }
        }
    }
}

            

                
