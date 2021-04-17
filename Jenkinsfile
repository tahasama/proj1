
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                ansiblePlaybook becomeUser: null, credentialsId: '69832d10-b9ae-4885-892a-5301ec83305b', disableHostKeyChecking: true, installation: 'ansible', playbook: 'play-ansible.yml', sudoUser: null                
                sh 'apache2 -version'
             
            }
            }
    }
}
