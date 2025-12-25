// ansiColor('xterm') {
//     ansiblePlaybook(
//         playbook: 'playbook.yml',
//         inventory: 'nventory.ini'
//         // colorized: true 
//         )
// }


steps {
    ansiblePlaybook('playbook.yml') {
        inventoryPath('nventory.ini')
        // ansibleName('1.9.4')
        tags('one,two')
        // credentialsId('credsid')
        become(true)
        becomeUser("user")
        checkMode(false)
        // extraVars {
        //     extraVar("key1", "value1", false)
        //     extraVar("key2", "value2", true)
        // }
    }
}