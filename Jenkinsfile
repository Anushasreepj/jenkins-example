pipeline {
    agent any
 parameters { 
     string(defaultValue: ')
  }          
    stages {
        stage ('Checkout') {
            steps {
                script {
                    def gitRepoUrl='
                }
            }

        stage ('build') {
            steps {
                withMaven(maven : 'mavenA') {
                    sh 'mvn clean'
                }
            }
        stage('Deploy to tomcat') {
            steps {
                script { 
                    def tomcatwebappsDir = "/home/ec2-user/apache-tomcat-8.5.93/webapps"
                    def warFilePath = "${tomcatwebappsDir}${gameoflife.war}"
                    if (fileExists(/home/ec2-user/apache-tomcat-8.5.93/webapps/gameoflife.war)) {
                        echo "Found existing ${war} in Tomcat's webapps directory."
                        echo"no need to deploy again."
                    } else {
                        error "could not found"
                    }
                }
            }
        }


    
