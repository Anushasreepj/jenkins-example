pipeline {
    agent any

    stages {
        stage('open application') {
            steps {
                script{
                      def tomcatUrl ='http://54.153.158.154:8088'
                      def contextPath ='/gameoflife'
                      sh "curl -u http://54.153.158.154:8088/gameoflife/"
                      def username ='manager'
                      def password ='manager'
                      sh "curl -u $username:$password $tomcatUrl$encodedContextPath" 
            }
        }
        }
    }
}



            

                
