pipeline {
    agent any

    stages {
        stage('open application') {
            steps {
                script{
                      def tomcatUrl ='http://54.153.158.154:8088'
                      def contextPath ='/gameoflife%20%281%29'
                      sh "curl http://54.153.158.154:8088/gameoflife (1).war"
                      def username ='manager'
                      def password ='manager'
                      sh "curl -u $username:$password $tomcatUrl$contexrPath" 
            }
        }
        }
    }
}



            

                
