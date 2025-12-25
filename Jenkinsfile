// ansiColor('xterm') {
//     ansiblePlaybook(
//         playbook: 'playbook.yml',
//         inventory: 'nventory.ini'
//         // colorized: true 
//         )
// }

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                ansiblePlaybook(
                    playbook: 'playbook.yml',
                    inventory: 'inventory.ini',
                    become: true,
                    becomeUser: 'user',
                    checkMode: false
                )
            }
       }
    }
}