currentBuild.displayName="Jenkins_20.1.0."+currentBuild.number
//env.BRANCH_NAME
pipeline{
    agent any
    environment{
        MVN_HOME = "/softwares/maven3/bin/mvn"
        //currentBuild.displayName="Jenkins_declarative-#"+currentBuild.number
    }
    stages{
        stage ("Maven Build"){
            steps{
                def branch = "${BRANCH_NAME}"
                sh "echo ${branch}"
                sh "${MVN_HOME} clean package"
                sh "mv target/*.war target/${currentBuild.displayName}.war"
                //sh "echo ${env.BRANCH_NAME}"
            }
        }
    }
}
