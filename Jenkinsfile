pipeline {
    agent any
 parameters { 
     string(defaultValue:'https://github.com/Anushasreepj/jenkins-example.git')
  }          
    stages {
        stage ('Checkout') {
            steps {
                script {
                    def gitRepoUrl=('https://github.com/Anushasreepj/jenkins-example.git)
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
                    def warFileName = "gameoflife.war"
                    def warFilePath ="${tomcatwebappsDir}${warFileName}"
                    if (fileExists(/home/ec2-user/apache-tomcat-8.5.93/webapps/gameoflife.war)) {
                        echo "Found existing ${gameoflife} in Tomcat's webapps directory."
                        bat "start \"\"\"${/home/ec2-user/apache-tomcat-8.5.93/webapp/gameoflife.war}\""
                    } else {
                        error "could not found"
                    }
                }
            }
        }


    
