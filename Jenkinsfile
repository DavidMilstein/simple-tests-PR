כככpipeline {

    agent any
    stages {

        stage('unit-test') {
            steps {
                bat(/mvn -Dthrow=false -fn clean test/)
            }
        }
    }

    post {
            always {
                echo 'I will always say Hello again! Einav!'
                junit '**/target/surefire-reports/TEST-*.xml'
            }
        }

}
