pipeline {
    agent any

    stages {
        stage('open application') {
            steps {
                script{
                      def tomcatUrl ='http://54.153.158.154:8088'
                      def contextPath ='/gameoflife (1).war'
                      def encodedContextPath = contextPath.replaceAll(' ','%20')
                      sh "curl -u http://54.153.158.154:8088/gameoflife%20(1)/"
                      def username ='manager'
                      def password ='manager'
                      sh "curl -u $username:$password $tomcatUrl$encodedContextPath" 
            }
        }
        }
    }
}



            

                
