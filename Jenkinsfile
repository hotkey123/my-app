pipeline{
    agent any
    stages{
        stage ("SCM checkout"){
            steps{
                git branch: 'Develop', credentialsId: 'git-creds', url: 'https://github.com/hotkey123/my-app.git'
            }
        }
    }
}
