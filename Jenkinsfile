pipeline{
    agent any
    environment{
        MVN_HOME = "/softwares/maven3/bin/mvn"
    }
    stages{
        stage ("Maven Build"){
            steps{
                sh "${MVN_HOME} clean package"
            }
        }
    }
}
