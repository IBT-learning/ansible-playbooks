pipeline {
    agent any
    stages {
        stage('Configurae VM with Tomcat') {
            steps {
               ansiblePlaybook(
                    playbook: 'tomcat.yaml',
                    inventory: 'hosts', 
                    credentialsId: 'vm-ssh',
                    colorized: true 
                    )
                }
            }
        }
}
