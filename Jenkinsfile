currentBuild.displayName="Jenkins_declarative-"+currentBuild.number
pipeline{
    agent any
    environment{
        MVN_HOME = "/softwares/maven3/bin/mvn"
        //currentBuild.displayName="Jenkins_declarative-#"+currentBuild.number
    }
    stages{
        stage ("Maven Build"){
            steps{
                sh "${MVN_HOME} clean package"
                sh "mv target/*.war target/${currentBuild.displayName}.war"
            }
        }
    }
}
