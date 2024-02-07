pipeline{
    agent{
        label "jenkins-agent"
    }
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace "){
            steps {
                cleanWs()

            }

          
        }
    }
    stages{
        stage("Checkout from SCM "){
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/Moetezafif-git/kubernetes-ci-cd'

            }

          
        }
    }
    
  
}