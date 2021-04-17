
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                ansiblePlaybook become: true, colorized: true, credentialsId: '69832d10-b9ae-4885-892a-5301ec83305b', disableHostKeyChecking: true, installation: 'ansible', playbook: 'play-ansible.yml'                
                sh 'apache2 -version'
             
            }
            }
    }
}
